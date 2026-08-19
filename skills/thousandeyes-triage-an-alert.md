---
name: thousandeyes-triage-an-alert
description: Triage a firing ThousandEyes alert end to end — list active alerts, open the alert, read the rule that fired, then pull the test results and path visualization that explain it.
api: ThousandEyes API v7
base_url: https://api.thousandeyes.com/v7
operations:
  - getAlerts
  - getAlert
  - getAlertsRules
  - getAlertRule
  - getTestNetworkResults
  - getTestPathVisResults
---

# Triage a ThousandEyes alert

Use this when something is firing and you need the shortest path from "an alert exists" to
"here is the hop that is losing packets".

## Before you start

- `Authorization: Bearer <token>` on every request. Tokens come from
  Manage > Account Settings > Users and Roles > Profile > User API Tokens and are shown once.
- If your user belongs to more than one account group, add `?aid=<accountGroupId>` to every
  call. Without it you are querying your login account group.
- Responses are JSON only. Errors are `application/problem+json` (RFC 9457).

## Steps

1. **List what is firing.** `getAlerts` — `GET /alerts`.
   Narrow with `window` (for example `window=2h`) or `startDate`/`endDate`. The response
   paginates: follow `_links.next.href` until it is absent.
2. **Open the alert.** `getAlert` — `GET /alerts/{alertId}`.
   This gives you `alert.rule.id`, `alert.test.id`, severity, first-seen and cleared times,
   and the affected agents or monitors.
3. **Read the rule.** `getAlertRule` — `GET /alerts/rules/{ruleId}`, or `getAlertsRules`
   (`GET /alerts/rules`) if you need to see the whole rule set. The `expression` field is the
   machine-readable condition that fired — quote it in the incident, not the rule name.
4. **Pull the measurement.** `getTestNetworkResults` — `GET /test-results/{testId}/network`
   with the same time window as the alert. Loss, latency and jitter per agent per round.
5. **Find the hop.** `getTestPathVisResults` — `GET /test-results/{testId}/path-vis`.
   Hop-by-hop path for each agent, which is what turns "the app is slow" into "AS 3356 hop 7".

## Rules to respect

- **Rate limit:** 240 requests per minute per organization. Watch
  `X-Organization-Rate-Limit-Remaining` and, on 429, wait until the UTC timestamp in
  `X-Organization-Rate-Limit-Reset`. There is no `Retry-After` header.
- **Time ranges:** use `window` (relative, e.g. `10d`, `2h`) OR `startDate` + `endDate`
  (absolute ISO 8601 UTC). Do not send both.
- **403 means permissions, not credentials.** The token is valid; the role lacks the
  operation's permission. 401 means the token is wrong or the account is locked.
