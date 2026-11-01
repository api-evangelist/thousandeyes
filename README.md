# ThousandEyes

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

ThousandEyes is Cisco's digital experience monitoring platform, acquired in 2020 and operated as part of Cisco Networking. It runs a global fleet of Cloud, Enterprise, Endpoint and Connected Device agents that measure network paths, BGP routing, DNS, application response and internet outages end to end, then exposes that telemetry through the ThousandEyes v7 REST API. The v7 API is documented on Cisco DevNet and publishes 26 downloadable OpenAPI 3.0 documents plus a unified document covering 326 operations across tests, instant tests, test results, agents, endpoint agents, alerts, event detection, dashboards, tags, templates, integrations, credentials, Internet Insights, Cloud Insights, usage and administration. Authentication is a bearer API token, with an OAuth 2.0 authorization-code and device-code flow advertised anonymously at /.well-known/oauth-authorization-server. Cisco also runs a remote MCP server at https://api.thousandeyes.com/mcp with about 51 documented tools, generated SDKs for Python, Java and Go, a Go CLI, a Terraform provider, a public Postman collection and a ThousandEyes for Government FedRAMP Moderate instance.

**Areas:** Monitoring · Network Visibility · Digital Experience · Observability · Networking · Enterprise · Synthetic Monitoring · BGP · Internet Insights · Endpoint Monitoring · OpenTelemetry · Cisco

## ThousandEyes on APIs.io

Everything profiled for ThousandEyes is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/thousandeyes/](https://apis.io/providers/thousandeyes/)** — or go straight to one of the APIs or properties below.

### APIs (98)

- [ThousandEyes Account Groups API](https://apis.io/apis/thousandeyes/thousandeyes-account-groups-api/) — Account group CRUD operations
- [ThousandEyes Agent Proxies API](https://apis.io/apis/thousandeyes/thousandeyes-agent-proxies-api/) — The Agent Proxies API from ThousandEyes — 1 operation(s) for agent proxies.
- [ThousandEyes Agent to Agent Instant Tests API](https://apis.io/apis/thousandeyes/thousandeyes-agent-to-agent-instant-tests-api/) — The Agent to Agent Instant Tests API from ThousandEyes — 1 operation(s) for agent to agent instant tests.
- [ThousandEyes Agent to Agent Tests API](https://apis.io/apis/thousandeyes/thousandeyes-agent-to-agent-tests-api/) — Agent to Agent test management operations
- [ThousandEyes Agent To Server Endpoint Dynamic Tests API](https://apis.io/apis/thousandeyes/thousandeyes-agent-to-server-endpoint-dynamic-tests-api/) — The Agent To Server Endpoint Dynamic Tests API from ThousandEyes — 2 operation(s) for agent to server endpoint dynamic tests.
- [ThousandEyes Agent to Server Endpoint Instant Scheduled Tests API](https://apis.io/apis/thousandeyes/thousandeyes-agent-to-server-endpoint-instant-scheduled-tests-api/) — The Agent to Server Endpoint Instant Scheduled Tests API from ThousandEyes — 1 operation(s) for agent to server endpoint instant scheduled tests.
- [ThousandEyes Agent to Server Endpoint Scheduled Tests API](https://apis.io/apis/thousandeyes/thousandeyes-agent-to-server-endpoint-scheduled-tests-api/) — The Agent to Server Endpoint Scheduled Tests API from ThousandEyes — 2 operation(s) for agent to server endpoint scheduled tests.
- [ThousandEyes Agent to Server Instant Tests API](https://apis.io/apis/thousandeyes/thousandeyes-agent-to-server-instant-tests-api/) — The Agent to Server Instant Tests API from ThousandEyes — 1 operation(s) for agent to server instant tests.
- [ThousandEyes Agent to Server Tests API](https://apis.io/apis/thousandeyes/thousandeyes-agent-to-server-tests-api/) — Agent to Server test management operations
- [ThousandEyes Alert Rules API](https://apis.io/apis/thousandeyes/thousandeyes-alert-rules-api/) — The Alert Rules API from ThousandEyes — 2 operation(s) for alert rules.
- [ThousandEyes Alert Suppression Windows API](https://apis.io/apis/thousandeyes/thousandeyes-alert-suppression-windows-api/) — The Alert Suppression Windows API from ThousandEyes — 2 operation(s) for alert suppression windows.
- [ThousandEyes Alerts API](https://apis.io/apis/thousandeyes/thousandeyes-alerts-api/) — The Alerts API from ThousandEyes — 2 operation(s) for alerts.
- [ThousandEyes API Instant Tests API](https://apis.io/apis/thousandeyes/thousandeyes-api-instant-tests-api/) — The API Instant Tests API from ThousandEyes — 1 operation(s) for api instant tests.
- [ThousandEyes API Test Results API](https://apis.io/apis/thousandeyes/thousandeyes-api-test-results-api/) — The API Test Results API from ThousandEyes — 2 operation(s) for api test results.
- [ThousandEyes API Tests API](https://apis.io/apis/thousandeyes/thousandeyes-api-tests-api/) — API test management operations
- [ThousandEyes API Token API](https://apis.io/apis/thousandeyes/thousandeyes-api-token-api/) — The API Token API from ThousandEyes — 1 operation(s) for api token.
- [ThousandEyes Autonomous System Prefixes API](https://apis.io/apis/thousandeyes/thousandeyes-autonomous-system-prefixes-api/) — The Autonomous System Prefixes API from ThousandEyes — 1 operation(s) for autonomous system prefixes.
- [ThousandEyes BGP monitors API](https://apis.io/apis/thousandeyes/thousandeyes-bgp-monitors-api/) — The BGP monitors API from ThousandEyes — 1 operation(s) for bgp monitors.
- [ThousandEyes BGP Tests API](https://apis.io/apis/thousandeyes/thousandeyes-bgp-tests-api/) — BGP test management operations
- [ThousandEyes Cloud and Enterprise Agent Notification Rules API](https://apis.io/apis/thousandeyes/thousandeyes-cloud-and-enterprise-agent-notification-rules-api/) — The Cloud and Enterprise Agent Notification Rules API from ThousandEyes — 2 operation(s) for cloud and enterprise agent notification rules.
- [ThousandEyes Cloud and Enterprise Agents API](https://apis.io/apis/thousandeyes/thousandeyes-cloud-and-enterprise-agents-api/) — The Cloud and Enterprise Agents API from ThousandEyes — 2 operation(s) for cloud and enterprise agents.
- [ThousandEyes Cloud Insights Integration Policy Settings API](https://apis.io/apis/thousandeyes/thousandeyes-cloud-insights-integration-policy-settings-api/) — Manage Cloud Insights integration policy settings for AWS and Azure.
- [ThousandEyes Cloud Insights Integrations API](https://apis.io/apis/thousandeyes/thousandeyes-cloud-insights-integrations-api/) — Manage Cloud Insights integrations for AWS and Azure.
- [ThousandEyes Credential Vault Operations API](https://apis.io/apis/thousandeyes/thousandeyes-credential-vault-operations-api/) — Credential Vault operations allow you to configure vault secrets.
- [ThousandEyes Credentials API](https://apis.io/apis/thousandeyes/thousandeyes-credentials-api/) — The Credentials API from ThousandEyes — 2 operation(s) for credentials.
- [ThousandEyes CyberArk Conjur Connectors API](https://apis.io/apis/thousandeyes/thousandeyes-cyberark-conjur-connectors-api/) — The CyberArk Conjur instance you want the ThousandEyes platform to integrate with.
- [ThousandEyes Dashboard Snapshots API](https://apis.io/apis/thousandeyes/thousandeyes-dashboard-snapshots-api/) — Dashboard Snapshots CRUD operations
- [ThousandEyes Dashboards API](https://apis.io/apis/thousandeyes/thousandeyes-dashboards-api/) — Dashboards and Widgets operations
- [ThousandEyes Dashboards Filters API](https://apis.io/apis/thousandeyes/thousandeyes-dashboards-filters-api/) — The Dashboards Filters API from ThousandEyes — 2 operation(s) for dashboards filters.
- [ThousandEyes DNS Server Instant Tests API](https://apis.io/apis/thousandeyes/thousandeyes-dns-server-instant-tests-api/) — The DNS Server Instant Tests API from ThousandEyes — 1 operation(s) for dns server instant tests.
- [ThousandEyes DNS Server Test Results API](https://apis.io/apis/thousandeyes/thousandeyes-dns-server-test-results-api/) — The DNS Server Test Results API from ThousandEyes — 2 operation(s) for dns server test results.
- [ThousandEyes DNS Server Tests API](https://apis.io/apis/thousandeyes/thousandeyes-dns-server-tests-api/) — DNS Server test management operations
- [ThousandEyes DNS Trace Instant Tests API](https://apis.io/apis/thousandeyes/thousandeyes-dns-trace-instant-tests-api/) — The DNS Trace Instant Tests API from ThousandEyes — 1 operation(s) for dns trace instant tests.
- [ThousandEyes DNS Trace Test Results API](https://apis.io/apis/thousandeyes/thousandeyes-dns-trace-test-results-api/) — The DNS Trace Test Results API from ThousandEyes — 1 operation(s) for dns trace test results.
- [ThousandEyes DNS Trace Tests API](https://apis.io/apis/thousandeyes/thousandeyes-dns-trace-tests-api/) — DNS Trace test management operations
- [ThousandEyes DNSSEC Instant Tests API](https://apis.io/apis/thousandeyes/thousandeyes-dnssec-instant-tests-api/) — The DNSSEC Instant Tests API from ThousandEyes — 1 operation(s) for dnssec instant tests.
- [ThousandEyes DNSSEC Test Results API](https://apis.io/apis/thousandeyes/thousandeyes-dnssec-test-results-api/) — The DNSSEC Test Results API from ThousandEyes — 1 operation(s) for dnssec test results.
- [ThousandEyes DNSSEC Tests API](https://apis.io/apis/thousandeyes/thousandeyes-dnssec-tests-api/) — DNSSEC test management operations
- [ThousandEyes Emulation API](https://apis.io/apis/thousandeyes/thousandeyes-emulation-api/) — The Emulation API from ThousandEyes — 2 operation(s) for emulation.
- [ThousandEyes Endpoint Agent Labels API](https://apis.io/apis/thousandeyes/thousandeyes-endpoint-agent-labels-api/) — The Endpoint Agent Labels API from ThousandEyes — 2 operation(s) for endpoint agent labels.
- [ThousandEyes Endpoint Agent Log Items API](https://apis.io/apis/thousandeyes/thousandeyes-endpoint-agent-log-items-api/) — The Endpoint Agent Log Items API from ThousandEyes — 1 operation(s) for endpoint agent log items.
- [ThousandEyes Endpoint Agents API](https://apis.io/apis/thousandeyes/thousandeyes-endpoint-agents-api/) — The Endpoint Agents API from ThousandEyes — 6 operation(s) for endpoint agents.
- [ThousandEyes Endpoint Agents Transfer API](https://apis.io/apis/thousandeyes/thousandeyes-endpoint-agents-transfer-api/) — The Endpoint Agents Transfer API from ThousandEyes — 2 operation(s) for endpoint agents transfer.
- [ThousandEyes Endpoint Proxies API](https://apis.io/apis/thousandeyes/thousandeyes-endpoint-proxies-api/) — The Endpoint Proxies API from ThousandEyes — 1 operation(s) for endpoint proxies.
- [ThousandEyes Endpoint Real User Tests API](https://apis.io/apis/thousandeyes/thousandeyes-endpoint-real-user-tests-api/) — The Endpoint Real User Tests API from ThousandEyes — 1 operation(s) for endpoint real user tests.
- [ThousandEyes Endpoint Scheduled Tests API](https://apis.io/apis/thousandeyes/thousandeyes-endpoint-scheduled-tests-api/) — The Endpoint Scheduled Tests API from ThousandEyes — 1 operation(s) for endpoint scheduled tests.
- [ThousandEyes Enterprise Agent Cluster API](https://apis.io/apis/thousandeyes/thousandeyes-enterprise-agent-cluster-api/) — The Enterprise Agent Cluster API from ThousandEyes — 2 operation(s) for enterprise agent cluster.
- [ThousandEyes Events API](https://apis.io/apis/thousandeyes/thousandeyes-events-api/) — The Events API from ThousandEyes — 2 operation(s) for events.
- [ThousandEyes FTP Server Instant Tests API](https://apis.io/apis/thousandeyes/thousandeyes-ftp-server-instant-tests-api/) — The FTP Server Instant Tests API from ThousandEyes — 1 operation(s) for ftp server instant tests.
- [ThousandEyes FTP Server Tests API](https://apis.io/apis/thousandeyes/thousandeyes-ftp-server-tests-api/) — FTP Server test management operations
- [ThousandEyes Generic Connectors API](https://apis.io/apis/thousandeyes/thousandeyes-generic-connectors-api/) — A generic connector represents an instance of a third-party service that you can integrate with the ThousandEyes platform.
- [ThousandEyes HTTP Page Load Instant Tests API](https://apis.io/apis/thousandeyes/thousandeyes-http-page-load-instant-tests-api/) — The HTTP Page Load Instant Tests API from ThousandEyes — 1 operation(s) for http page load instant tests.
- [ThousandEyes HTTP Server Endpoint Instant Scheduled Tests API](https://apis.io/apis/thousandeyes/thousandeyes-http-server-endpoint-instant-scheduled-tests-api/) — The HTTP Server Endpoint Instant Scheduled Tests API from ThousandEyes — 1 operation(s) for http server endpoint instant scheduled tests.
- [ThousandEyes HTTP Server Endpoint Scheduled Test Results API](https://apis.io/apis/thousandeyes/thousandeyes-http-server-endpoint-scheduled-test-results-api/) — The HTTP Server Endpoint Scheduled Test Results API from ThousandEyes — 3 operation(s) for http server endpoint scheduled test results.
- [ThousandEyes HTTP Server Endpoint Scheduled Tests API](https://apis.io/apis/thousandeyes/thousandeyes-http-server-endpoint-scheduled-tests-api/) — The HTTP Server Endpoint Scheduled Tests API from ThousandEyes — 2 operation(s) for http server endpoint scheduled tests.
- [ThousandEyes HTTP Server Instant Tests API](https://apis.io/apis/thousandeyes/thousandeyes-http-server-instant-tests-api/) — The HTTP Server Instant Tests API from ThousandEyes — 1 operation(s) for http server instant tests.
- [ThousandEyes HTTP Server Tests API](https://apis.io/apis/thousandeyes/thousandeyes-http-server-tests-api/) — HTTP Server test management operations
- [ThousandEyes Instant Tests API](https://apis.io/apis/thousandeyes/thousandeyes-instant-tests-api/) — The Instant Tests API from ThousandEyes — 1 operation(s) for instant tests.
- [ThousandEyes Internet Insights Catalog Providers API](https://apis.io/apis/thousandeyes/thousandeyes-internet-insights-catalog-providers-api/) — The Internet Insights Catalog Providers API from ThousandEyes — 2 operation(s) for internet insights catalog providers.
- [ThousandEyes Internet Insights Outages API](https://apis.io/apis/thousandeyes/thousandeyes-internet-insights-outages-api/) — The Internet Insights Outages API from ThousandEyes — 3 operation(s) for internet insights outages.
- [ThousandEyes Local Network Endpoint Test Results API](https://apis.io/apis/thousandeyes/thousandeyes-local-network-endpoint-test-results-api/) — The Local Network Endpoint Test Results API from ThousandEyes — 3 operation(s) for local network endpoint test results.
- [ThousandEyes Local Problems API](https://apis.io/apis/thousandeyes/thousandeyes-local-problems-api/) — The Local Problems API from ThousandEyes — 1 operation(s) for local problems.
- [ThousandEyes Network BGP Test Results API](https://apis.io/apis/thousandeyes/thousandeyes-network-bgp-test-results-api/) — The Network BGP Test Results API from ThousandEyes — 2 operation(s) for network bgp test results.
- [ThousandEyes Network Dynamic Endpoint Test Results API](https://apis.io/apis/thousandeyes/thousandeyes-network-dynamic-endpoint-test-results-api/) — The Network Dynamic Endpoint Test Results API from ThousandEyes — 3 operation(s) for network dynamic endpoint test results.
- [ThousandEyes Network Endpoint Scheduled Test Results API](https://apis.io/apis/thousandeyes/thousandeyes-network-endpoint-scheduled-test-results-api/) — The Network Endpoint Scheduled Test Results API from ThousandEyes — 4 operation(s) for network endpoint scheduled test results.
- [ThousandEyes Network Test Results API](https://apis.io/apis/thousandeyes/thousandeyes-network-test-results-api/) — The Network Test Results API from ThousandEyes — 3 operation(s) for network test results.
- [ThousandEyes Operation Connectors API](https://apis.io/apis/thousandeyes/thousandeyes-operation-connectors-api/) — Manage the connectors assigned to an operation.
- [ThousandEyes Page Load Tests API](https://apis.io/apis/thousandeyes/thousandeyes-page-load-tests-api/) — Page Load test management operations
- [ThousandEyes Panorama Connectors API](https://apis.io/apis/thousandeyes/thousandeyes-panorama-connectors-api/) — A Panorama connector represents an instance of Palo Alto Networks Panorama that you can integrate with the ThousandEyes platform.
- [ThousandEyes Path Visualization Interface Groups API](https://apis.io/apis/thousandeyes/thousandeyes-path-visualization-interface-groups-api/) — The Path Visualization Interface Groups API from ThousandEyes — 2 operation(s) for path visualization interface groups.
- [ThousandEyes Permissions API](https://apis.io/apis/thousandeyes/thousandeyes-permissions-api/) — Permission GET operation
- [ThousandEyes Quotas API](https://apis.io/apis/thousandeyes/thousandeyes-quotas-api/) — Quota CRUD Operation
- [ThousandEyes Real User Endpoint Test Results API](https://apis.io/apis/thousandeyes/thousandeyes-real-user-endpoint-test-results-api/) — The Real User Endpoint Test Results API from ThousandEyes — 5 operation(s) for real user endpoint test results.
- [ThousandEyes Roles API](https://apis.io/apis/thousandeyes/thousandeyes-roles-api/) — Role CRUD operations
- [ThousandEyes Run Endpoint Instant Scheduled Tests API](https://apis.io/apis/thousandeyes/thousandeyes-run-endpoint-instant-scheduled-tests-api/) — The Run Endpoint Instant Scheduled Tests API from ThousandEyes — 1 operation(s) for run endpoint instant scheduled tests.
- [ThousandEyes SIP Server Instant Tests API](https://apis.io/apis/thousandeyes/thousandeyes-sip-server-instant-tests-api/) — The SIP Server Instant Tests API from ThousandEyes — 1 operation(s) for sip server instant tests.
- [ThousandEyes SIP Server Tests API](https://apis.io/apis/thousandeyes/thousandeyes-sip-server-tests-api/) — SIP Server test management operations
- [ThousandEyes Streaming API](https://apis.io/apis/thousandeyes/thousandeyes-streaming-api/) — Configure data streaming
- [ThousandEyes Tag Assignment API](https://apis.io/apis/thousandeyes/thousandeyes-tag-assignment-api/) — Assign tags to other objects
- [ThousandEyes Tags API](https://apis.io/apis/thousandeyes/thousandeyes-tags-api/) — Tag CRUD Operations
- [ThousandEyes Templates API](https://apis.io/apis/thousandeyes/thousandeyes-templates-api/) — The Templates API from ThousandEyes — 4 operation(s) for templates.
- [ThousandEyes Test Snapshots API](https://apis.io/apis/thousandeyes/thousandeyes-test-snapshots-api/) — The Test Snapshots API from ThousandEyes — 1 operation(s) for test snapshots.
- [ThousandEyes Tests API](https://apis.io/apis/thousandeyes/thousandeyes-tests-api/) — Get all tests
- [ThousandEyes Tests Assignment on Agents API](https://apis.io/apis/thousandeyes/thousandeyes-tests-assignment-on-agents-api/) — The Tests Assignment on Agents API from ThousandEyes — 3 operation(s) for tests assignment on agents.
- [ThousandEyes Usage API](https://apis.io/apis/thousandeyes/thousandeyes-usage-api/) — Usage GET Operation
- [ThousandEyes User Events API](https://apis.io/apis/thousandeyes/thousandeyes-user-events-api/) — User events GET operation
- [ThousandEyes Users API](https://apis.io/apis/thousandeyes/thousandeyes-users-api/) — User CRUD operations
- [ThousandEyes Voice Instant Tests API](https://apis.io/apis/thousandeyes/thousandeyes-voice-instant-tests-api/) — The Voice Instant Tests API from ThousandEyes — 1 operation(s) for voice instant tests.
- [ThousandEyes Voice RTP Server Test Results API](https://apis.io/apis/thousandeyes/thousandeyes-voice-rtp-server-test-results-api/) — The Voice RTP Server Test Results API from ThousandEyes — 1 operation(s) for voice rtp server test results.
- [ThousandEyes Voice SIP Server Test Results API](https://apis.io/apis/thousandeyes/thousandeyes-voice-sip-server-test-results-api/) — The Voice SIP Server Test Results API from ThousandEyes — 1 operation(s) for voice sip server test results.
- [ThousandEyes Voice Tests API](https://apis.io/apis/thousandeyes/thousandeyes-voice-tests-api/) — Voice test management operations
- [ThousandEyes Web FTP Server Test Results API](https://apis.io/apis/thousandeyes/thousandeyes-web-ftp-server-test-results-api/) — The Web FTP Server Test Results API from ThousandEyes — 1 operation(s) for web ftp server test results.
- [ThousandEyes Web HTTP Server Test Results API](https://apis.io/apis/thousandeyes/thousandeyes-web-http-server-test-results-api/) — The Web HTTP Server Test Results API from ThousandEyes — 1 operation(s) for web http server test results.
- [ThousandEyes Web Page Load Test Results API](https://apis.io/apis/thousandeyes/thousandeyes-web-page-load-test-results-api/) — The Web Page Load Test Results API from ThousandEyes — 2 operation(s) for web page load test results.
- [ThousandEyes Web Transaction Instant Tests API](https://apis.io/apis/thousandeyes/thousandeyes-web-transaction-instant-tests-api/) — The Web Transaction Instant Tests API from ThousandEyes — 1 operation(s) for web transaction instant tests.
- [ThousandEyes Web Transaction Tests API](https://apis.io/apis/thousandeyes/thousandeyes-web-transaction-tests-api/) — Web Transactions test management operations
- [ThousandEyes Web Transactions Test Results API](https://apis.io/apis/thousandeyes/thousandeyes-web-transactions-test-results-api/) — The Web Transactions Test Results API from ThousandEyes — 4 operation(s) for web transactions test results.
- [ThousandEyes Webhook Operations API](https://apis.io/apis/thousandeyes/thousandeyes-webhook-operations-api/) — Webhook operations allow you to customize the payload of generic connectors.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### AsyncAPI (1)

Event-driven and webhook contracts.

- [Thousandeyes Webhooks](https://apis.io/asyncapis/thousandeyes/thousandeyes-webhooks/)

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [ThousandEyes MCP Server](https://apis.io/servers/thousandeyes/thousandeyes-mcp-server/)

#### Overlays (124)

OpenAPI overlays, including conversational phrasing for each operation.

- [Thousandeyes Account Groups Api Phrasing Overlay](https://apis.io/overlays/thousandeyes/thousandeyes-account-groups-api-phrasing-overlay/)
- [Thousandeyes Administrative Overlay](https://apis.io/overlays/thousandeyes/thousandeyes-administrative-overlay/)
- [Thousandeyes Agent Proxies Api Phrasing Overlay](https://apis.io/overlays/thousandeyes/thousandeyes-agent-proxies-api-phrasing-overlay/)
- [Thousandeyes Agent To Agent Instant Tests Api Phrasing Overlay](https://apis.io/overlays/thousandeyes/thousandeyes-agent-to-agent-instant-tests-api-phrasing-overlay/)
- [Thousandeyes Agent To Agent Tests Api Phrasing Overlay](https://apis.io/overlays/thousandeyes/thousandeyes-agent-to-agent-tests-api-phrasing-overlay/)
- [Thousandeyes Agent To Server Endpoint Dynamic Tests Api Phrasing Overlay](https://apis.io/overlays/thousandeyes/thousandeyes-agent-to-server-endpoint-dynamic-tests-api-phrasing-overlay/)
- [Thousandeyes Agent To Server Endpoint Instant Scheduled Tests Api Phrasing Overlay](https://apis.io/overlays/thousandeyes/thousandeyes-agent-to-server-endpoint-instant-scheduled-tests-api-phrasing-overlay/)
- [Thousandeyes Agent To Server Endpoint Scheduled Tests Api Phrasing Overlay](https://apis.io/overlays/thousandeyes/thousandeyes-agent-to-server-endpoint-scheduled-tests-api-phrasing-overlay/)
- [Thousandeyes Agent To Server Instant Tests Api Phrasing Overlay](https://apis.io/overlays/thousandeyes/thousandeyes-agent-to-server-instant-tests-api-phrasing-overlay/)
- [Thousandeyes Agent To Server Tests Api Phrasing Overlay](https://apis.io/overlays/thousandeyes/thousandeyes-agent-to-server-tests-api-phrasing-overlay/)
- [Thousandeyes Agents Overlay](https://apis.io/overlays/thousandeyes/thousandeyes-agents-overlay/)
- [Thousandeyes Alert Rules Api Phrasing Overlay](https://apis.io/overlays/thousandeyes/thousandeyes-alert-rules-api-phrasing-overlay/)
- [Thousandeyes Alert Suppression Windows Api Phrasing Overlay](https://apis.io/overlays/thousandeyes/thousandeyes-alert-suppression-windows-api-phrasing-overlay/)
- [Thousandeyes Alerts Api Phrasing Overlay](https://apis.io/overlays/thousandeyes/thousandeyes-alerts-api-phrasing-overlay/)
- [Thousandeyes Alerts Overlay](https://apis.io/overlays/thousandeyes/thousandeyes-alerts-overlay/)
- [Thousandeyes Api Instant Tests Api Phrasing Overlay](https://apis.io/overlays/thousandeyes/thousandeyes-api-instant-tests-api-phrasing-overlay/)
- [Thousandeyes Api Test Results Api Phrasing Overlay](https://apis.io/overlays/thousandeyes/thousandeyes-api-test-results-api-phrasing-overlay/)
- [Thousandeyes Api Tests Api Phrasing Overlay](https://apis.io/overlays/thousandeyes/thousandeyes-api-tests-api-phrasing-overlay/)
- [Thousandeyes Api Token Api Phrasing Overlay](https://apis.io/overlays/thousandeyes/thousandeyes-api-token-api-phrasing-overlay/)
- [Thousandeyes Api Token Management Overlay](https://apis.io/overlays/thousandeyes/thousandeyes-api-token-management-overlay/)
- [Thousandeyes Autonomous System Prefixes Api Phrasing Overlay](https://apis.io/overlays/thousandeyes/thousandeyes-autonomous-system-prefixes-api-phrasing-overlay/)
- [Thousandeyes Autonomous Systems Overlay](https://apis.io/overlays/thousandeyes/thousandeyes-autonomous-systems-overlay/)
- [Thousandeyes Bgp Monitors Api Phrasing Overlay](https://apis.io/overlays/thousandeyes/thousandeyes-bgp-monitors-api-phrasing-overlay/)
- [Thousandeyes Bgp Monitors Overlay](https://apis.io/overlays/thousandeyes/thousandeyes-bgp-monitors-overlay/)
- [Thousandeyes Bgp Tests Api Phrasing Overlay](https://apis.io/overlays/thousandeyes/thousandeyes-bgp-tests-api-phrasing-overlay/)
- …and 99 more published on APIs.io

#### Security (4)

Authentication, trust centre, and vulnerability disclosure.

- [Thousandeyes Authentication](https://apis.io/security/thousandeyes/thousandeyes-authentication/)
- [Thousandeyes Domain Security](https://apis.io/security/thousandeyes/thousandeyes-domain-security/)
- [Thousandeyes Trust Center](https://apis.io/security/thousandeyes/thousandeyes-trust-center/)
- [Thousandeyes Vulnerability Disclosure](https://apis.io/security/thousandeyes/thousandeyes-vulnerability-disclosure/)

#### OAuth scopes (1)

The permissions the API asks for.

- [Thousandeyes Scopes](https://apis.io/scopes/thousandeyes/thousandeyes-scopes/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Thousandeyes Plans Pricing](https://apis.io/plans/thousandeyes/thousandeyes-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [Thousandeyes Rate Limits](https://apis.io/rate-limits/thousandeyes/thousandeyes-rate-limits/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.thousandeyes.com/)
- [Documentation](https://docs.thousandeyes.com/)
- [Getting started](https://developer.cisco.com/docs/thousandeyes/getting-started/)
- [API reference](https://developer.cisco.com/docs/thousandeyes/)
- [Pricing](https://www.cisco.com/c/en/us/products/collateral/security/cisco-thousandeyes-og.html)
- [Sign up](https://app.thousandeyes.com/login?fwd=%2Fsignup)
- [Support](https://developer.cisco.com/docs/thousandeyes/developer-support/)
- [Blog](https://blogs.cisco.com/tag/cisco-thousandeyes)
- [Security](https://sec.cloudapps.cisco.com/security/center/resources/security_vulnerability_policy.html)
- [Compliance](https://trustportal.cisco.com/c/r/ctp/trust-portal.html)
- [Terms of service](https://developer.cisco.com/site/license/terms-and-conditions/)
- [Privacy policy](https://www.cisco.com/c/en/us/about/legal/privacy-full.html)
- [GitHub](https://github.com/thousandeyes)
- [Status](https://status.thousandeyes.com)

## API Evangelist rating

**Kin Score 75.6** — exemplar · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 80.0 |
| Contract quality | 63.0 |
| Contract governance | 4.5 |
| Operational transparency | 92.1 |
| Developer ergonomics | 75.6 |
| Access clarity | 85.5 |

**Agent readiness 55.3** — agent-ready (gated down from agent-native)

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | — |
| Reversibility Documented | — |
| MCP Server | verified |
| Auth Clarity | served (partial credit) |
| Idempotency | — |
| Error Semantics | verified |
| OpenAPI Examples | partial |
| Rate Limit Signal | documented (partial credit) |
| Event Surface Described | yes |
| Agent Skills | derived (partial credit) |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | served (partial credit) |
| Protected Resource Metadata | verified |
| Dynamic Client Registration | yes |
| Agentic Commerce | — |
| Pagination Ratio | — |
| Operation Distinctiveness | distinct |

**Regulatory alignment 45.1** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/thousandeyes/](https://apis.io/providers/thousandeyes/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for ThousandEyes: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/thousandeyes/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
