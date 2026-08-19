---
name: thousandeyes-stand-up-a-synthetic-test
description: Create a monitored HTTP or agent-to-server synthetic test on ThousandEyes — pick agents, create the test, tag it, attach an alert rule, then read the first results.
api: ThousandEyes API v7
base_url: https://api.thousandeyes.com/v7
operations:
  - getAgents
  - createHttpServerTest
  - createAgentToServerTest
  - getTests
  - createTag
  - assignTags
  - createAlertRule
  - getTestHttpServerResults
---

# Stand up a ThousandEyes synthetic test

## Before you start

- Bearer token in `Authorization`. Write operations need the `Settings Tests Update`
  permission; reads need `Settings Tests Read`.
- Add `?aid=<accountGroupId>` if your user spans multiple account groups.
- **There is no idempotency key.** A retried `POST /tests/...` creates a second test.
  If a create times out, call `getTests` and check before retrying.

## Steps

1. **Choose vantage points.** `getAgents` — `GET /agents`. Filter to the Cloud or
   Enterprise Agents you want; keep their `agentId` values.
2. **Create the test.**
   - Web/application target: `createHttpServerTest` — `POST /tests/http-server`.
   - Network reachability to a host and port: `createAgentToServerTest` —
     `POST /tests/agent-to-server`.
   Both take `agents[]` (the ids from step 1), an `interval`, and the target. The request
   body schema is in `openapi/thousandeyes-tests-openapi.yml`.
3. **Tag it.** `createTag` — `POST /tags` (key/value, e.g. `team:neteng`), then
   `assignTags` — `POST /tags/assign` to bind the tag to the new `testId`. Tags are the
   platform-wide metadata mechanism; use them instead of encoding meaning in test names.
4. **Alert on it.** `createAlertRule` — `POST /alerts/rules` with an `expression`,
   `alertType`, `severity` and violation window, and `testIds` containing the new test.
5. **Read results.** `getTestHttpServerResults` —
   `GET /test-results/{testId}/http-server?window=1h`. Nothing appears until the test has
   run at least one round at its configured interval.

## Rules to respect

- **Test types are separate endpoints.** There is no generic "create a test" operation —
  `/tests/http-server`, `/tests/agent-to-server`, `/tests/bgp`, `/tests/dns-server`, and so
  on each have their own create/read/update/delete operations.
- **Instant tests are a different API.** For a one-off run during troubleshooting use
  `POST /tests/http-server/instant` (`createHttpServerInstantTest`), which is rate limited
  separately at 24 requests per minute (`X-Instant-Test-Rate-Limit-*`).
- **Government instance:** page load, web transaction and API tests are not available on
  ThousandEyes for Government.
