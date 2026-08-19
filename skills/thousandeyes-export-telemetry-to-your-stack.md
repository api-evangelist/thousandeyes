---
name: thousandeyes-export-telemetry-to-your-stack
description: Get ThousandEyes data out — stand up an OpenTelemetry data stream for metrics and traces, or wire an outbound alert webhook through the Integrations API.
api: ThousandEyes API v7
base_url: https://api.thousandeyes.com/v7
operations:
  - getStreams
  - createStream
  - getStream
  - updateStream
  - deleteStream
  - getWebhookOperations
  - createWebhookOperation
  - getGenericConnectors
  - createGenericConnector
  - setOperationConnectors
---

# Export ThousandEyes telemetry to your own stack

Two mechanisms, and they are not interchangeable. Streams are a continuous push of
measurement data. Webhooks are event-driven notifications when an alert rule fires.

## Path A — OpenTelemetry data stream (metrics and traces)

1. `getStreams` — `GET /streams` to see what already exists.
2. `createStream` — `POST /streams` with the stream type (`opentelemetry`), the target
   endpoint URL, and the signal configuration under `inputConfig`. Since API 7.0.100 you
   can supply an optional durable `name`; omit it and one is generated.
3. `getStream` / `updateStream` / `deleteStream` — `GET|PUT|DELETE /streams/{id}`.

**Watch for:** a duplicate `name` on update returns **409 Conflict**. Streams that keep
failing are disabled automatically. Traces, Connected Devices metrics and connector-based
OTel integrations are unavailable on ThousandEyes for Government.

## Path B — outbound alert webhook

1. Create or pick a connector — `GET /connectors/generic`, `POST /connectors/generic`
   (also `panorama` for Palo Alto Networks and `conjur` for CyberArk).
2. Create the webhook operation — `POST /operations/webhooks`, with the destination URL,
   request headers, and the JSON body. **The body is a Handlebars template you author**, so
   the payload shape is yours, not ThousandEyes'. Variables include `alert.id`,
   `alert.severity.id`, `alert.rule.expression`, `alert.test.name` and `type.id`
   (1 = clear, 2 = trigger).
3. Bind the operation to a connector — `PUT /operations/{type}/{id}/connectors`.
4. Attach alert rules to the webhook in the app, then test the delivery.

**Watch for:** webhooks — including custom webhooks — are **not available** on
ThousandEyes for Government for alert notifications. Webhook authentication can be static
headers or OAuth 2.0 client credentials.

## Rules to respect

- Both paths are configuration APIs; the 240 requests/minute organization limit applies.
- There is no idempotency key. Re-POSTing a stream or webhook operation creates a second one.
- Since the webhook payload is operator-authored, no AsyncAPI or fixed message schema exists
  for it. Treat your template as the contract and version it on your side.
