# Freestyle

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

Freestyle is the infrastructure for code you didn't write — VMs and Git for AI agents. The platform provides Linux microVMs that boot in under 600ms with live-fork, pause-resume, and persistent snapshots; a multi-tenant Git service with branchable filesystems, GitHub Sync, full-text search, and webhook triggers; an Execute (Serverless Runs) API for ephemeral JavaScript/TypeScript code; a Web Deployments API for hosted Node.js apps and static sites; Cron schedules; custom Domains with wildcard SSL; an Identity service for scoped per-user and per-agent access tokens; and Observability logs. Freestyle is a direct sandbox option for AI app builders, background agents, code review bots, and long-running assistants — a usage-priced alternative to running Anthropic's hosted Code Execution tool or building bespoke microVM infrastructure on Firecracker, Modal, or E2B.

**Areas:** Artificial Intelligence · Agents · Sandbox · VMs · MicroVM · Version Control · Code Execution · JavaScript · TypeScript · Serverless · Hosting · Developer Tools

## Freestyle on APIs.io

Everything profiled for Freestyle is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/freestyle-sh/](https://apis.io/providers/freestyle-sh/)** — or go straight to one of the APIs or properties below.

### APIs (11)

- [Freestyle Auth API](https://apis.io/apis/freestyle-sh/freestyle-sh-auth-api/) — The Auth API from Freestyle — 2 operation(s) for auth.
- [Freestyle Certs API](https://apis.io/apis/freestyle-sh/freestyle-sh-certs-api/) — APIs for managing SSL certificates.
- [Freestyle Cron API](https://apis.io/apis/freestyle-sh/freestyle-sh-cron-api/) — The Cron API from Freestyle — 5 operation(s) for cron.
- [Freestyle DNS API](https://apis.io/apis/freestyle-sh/freestyle-sh-dns-api/) — APIs for managing DNS records.
- [Freestyle Domains API](https://apis.io/apis/freestyle-sh/freestyle-sh-domains-api/) — APIs for managing domains. This is only relevant when you want to start to deploy to custom domains. Please read [this…
- [Freestyle Execute API](https://apis.io/apis/freestyle-sh/freestyle-sh-execute-api/) — APIs for running code. Send the code using the [execute](#tag/execute/POST/execute/v1/execute) endpoint, and you'll get the output back. Works with any…
- [Freestyle Git API](https://apis.io/apis/freestyle-sh/freestyle-sh-git-api/) — APIs for managing git repositories and accessing git objects like commits, trees, blobs, tags, and refs.
- [Freestyle Identity API](https://apis.io/apis/freestyle-sh/freestyle-sh-identity-api/) — APIs for managing identities and access tokens.
- [Freestyle Observability API](https://apis.io/apis/freestyle-sh/freestyle-sh-observability-api/) — APIs for observability.
- [Freestyle VM API](https://apis.io/apis/freestyle-sh/freestyle-sh-vm-api/) — APIs for managing lightweight virtual machines (VMs) to run your code in isolated environments.
- [Freestyle Web API](https://apis.io/apis/freestyle-sh/freestyle-sh-web-api/) — APIs for deploying websites. We handle node modules caching, scaling, certificates and the whole end to end process. Send the code using the…

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Freestyle Sh Agentic Access](https://apis.io/agentic-access/freestyle-sh/freestyle-sh-agentic-access/)

#### JSON Schema (2)

The data models the API reads and writes.

- [Freestyle Repository](https://apis.io/schemas/freestyle-sh/freestyle-repository/)
- [Freestyle VM](https://apis.io/schemas/freestyle-sh/freestyle-vm/)

#### JSON-LD (1)

Linked-data contexts for the provider's vocabulary.

- [Freestyle Sh Context](https://apis.io/jsonld/freestyle-sh/freestyle-sh-context/)

#### Collections (30)

Postman and Open Collection request collections.

- [Freestyle Cron API](https://apis.io/collections/freestyle-sh/open-freestyle-cron-api/)
- [Freestyle Domains API](https://apis.io/collections/freestyle-sh/open-freestyle-domains-api/)
- [Freestyle Execute API](https://apis.io/collections/freestyle-sh/open-freestyle-execute-api/)
- [Freestyle Git API](https://apis.io/collections/freestyle-sh/open-freestyle-git-api/)
- [Freestyle Identity API](https://apis.io/collections/freestyle-sh/open-freestyle-identity-api/)
- [Freestyle Observability API](https://apis.io/collections/freestyle-sh/open-freestyle-observability-api/)
- [Freestyle Cron Auth API](https://apis.io/collections/freestyle-sh/open-freestyle-sh-auth-api/)
- [Freestyle Cron Auth Certs API](https://apis.io/collections/freestyle-sh/open-freestyle-sh-certs-api/)
- [Freestyle Auth Cron API](https://apis.io/collections/freestyle-sh/open-freestyle-sh-cron-api/)
- [Freestyle Cron Auth DNS API](https://apis.io/collections/freestyle-sh/open-freestyle-sh-dns-api/)
- [Freestyle Cron Auth Domains API](https://apis.io/collections/freestyle-sh/open-freestyle-sh-domains-api/)
- [Freestyle Cron Auth Execute API](https://apis.io/collections/freestyle-sh/open-freestyle-sh-execute-api/)
- [Freestyle Cron Auth Git API](https://apis.io/collections/freestyle-sh/open-freestyle-sh-git-api/)
- [Freestyle Cron Auth Identity API](https://apis.io/collections/freestyle-sh/open-freestyle-sh-identity-api/)
- [Freestyle Cron Auth Observability API](https://apis.io/collections/freestyle-sh/open-freestyle-sh-observability-api/)
- [Freestyle Cron Auth VM API](https://apis.io/collections/freestyle-sh/open-freestyle-sh-vm-api/)
- [Freestyle Cron Auth Web API](https://apis.io/collections/freestyle-sh/open-freestyle-sh-web-api/)
- [Freestyle VMs API](https://apis.io/collections/freestyle-sh/open-freestyle-vm-api/)
- [Freestyle Web Deployments API](https://apis.io/collections/freestyle-sh/open-freestyle-web-api/)
- [Freestyle Cron Auth API](https://apis.io/collections/freestyle-sh/postman-freestyle-sh-auth-api/)
- [Freestyle Cron Auth Certs API](https://apis.io/collections/freestyle-sh/postman-freestyle-sh-certs-api/)
- [Freestyle Auth Cron API](https://apis.io/collections/freestyle-sh/postman-freestyle-sh-cron-api/)
- [Freestyle Cron Auth DNS API](https://apis.io/collections/freestyle-sh/postman-freestyle-sh-dns-api/)
- [Freestyle Cron Auth Domains API](https://apis.io/collections/freestyle-sh/postman-freestyle-sh-domains-api/)
- [Freestyle Cron Auth Execute API](https://apis.io/collections/freestyle-sh/postman-freestyle-sh-execute-api/)
- …and 5 more published on APIs.io

#### Governance rules (1)

Spectral rulesets for the provider's contracts.

- [Freestyle — jsonschema rules](https://apis.io/rules/freestyle-sh/freestyle-sh-jsonschema-spectral-rules/)

#### Security (2)

Authentication, trust centre, and vulnerability disclosure.

- [Freestyle Sh Authentication](https://apis.io/security/freestyle-sh/freestyle-sh-authentication/)
- [Freestyle Sh Domain Security](https://apis.io/security/freestyle-sh/freestyle-sh-domain-security/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Freestyle Sh Plans Pricing](https://apis.io/plans/freestyle-sh/freestyle-sh-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [Freestyle Sh Rate Limits](https://apis.io/rate-limits/freestyle-sh/freestyle-sh-rate-limits/)

#### FinOps (1)

What the API costs to run, by operation.

- [Freestyle Sh Finops](https://apis.io/finops/freestyle-sh/freestyle-sh-finops/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.freestyle.sh/)
- [Documentation](https://docs.freestyle.sh)
- [Getting started](https://docs.freestyle.sh/v2/about)
- [Pricing](https://www.freestyle.sh/pricing)
- [Blog](https://www.freestyle.sh/blog)
- [Privacy policy](https://www.freestyle.sh/privacy)
- [GitHub](https://github.com/freestyle-sh)
- [Status](https://status.freestyle.sh)

## API Evangelist rating

**Kin Score 51.3** — developing · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 62.5 |
| Contract quality | 66.7 |
| Contract governance | 9.8 |
| Operational transparency | 28.9 |
| Developer ergonomics | 67.9 |
| Access clarity | 50.0 |

**Agent readiness 26.4** — agent-aware

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | documented (partial credit) |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
| Idempotency | — |
| Error Semantics | verified |
| OpenAPI Examples | partial |
| Rate Limit Signal | derived (partial credit) |
| Event Surface Described | — |
| Agent Skills | — |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |
| Pagination Ratio | — |
| Operation Distinctiveness | — |

**Regulatory alignment 19.1** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/freestyle-sh/](https://apis.io/providers/freestyle-sh/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Freestyle: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/freestyle-sh/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
