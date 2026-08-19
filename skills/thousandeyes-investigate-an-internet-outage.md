---
name: thousandeyes-investigate-an-internet-outage
description: Work out whether a problem is yours or the internet's — search Internet Insights outages, read the outage detail, then correlate with detected events and BGP routing.
api: ThousandEyes API v7
base_url: https://api.thousandeyes.com/v7
operations:
  - filterOutages
  - getNetworkOutage
  - getAppOutage
  - getEvents
  - getEvent
  - getTestBgpResults
  - getTestBgpRoutesPrefixRoundResults
---

# Investigate an internet outage

The question this answers: *is this us, our provider, or the internet?*

## Steps

1. **Search outages.** `filterOutages` — `POST /internet-insights/outages/filter`.
   The filter body takes a time window plus provider, region and application constraints.
   This is a POST because the filter is a document, not a query string.
2. **Open the outage.**
   - Network-layer: `getNetworkOutage` — `GET /internet-insights/outages/net/{outageId}`.
   - Application-layer: `getAppOutage` — `GET /internet-insights/outages/app/{outageId}`.
   You get affected locations, ASNs, providers and the duration.
3. **Correlate with your own estate.** `getEvents` — `GET /events` for the same window,
   then `getEvent` — `GET /events/{id}` on anything that overlaps. Events are
   ThousandEyes' own baseline-deviation detections across your tests, so an event that
   lines up with a public outage is your confirmation.
4. **Check routing.** If the outage is network-layer, `getTestBgpResults` —
   `GET /test-results/{testId}/bgp` on a BGP test for the affected prefix, then
   `getTestBgpRoutesPrefixRoundResults` —
   `GET /test-results/{testId}/bgp/routes/prefix/{prefixId}/round/{roundId}` for the AS path
   at the round where it changed.

## Rules to respect

- **Internet Insights is licensed separately** and is not available on ThousandEyes for
  Government. A 403 here can mean "not entitled", not "wrong token".
- Use the **same window** at every step. Mixing `window` at one step and
  `startDate`/`endDate` at the next is the most common way to conclude nothing correlates.
- Outage searches paginate like everything else — follow `_links.next.href`.
