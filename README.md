# Freestyle (freestyle-sh)

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
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Freestyle is the infrastructure for code you didn't write — VMs and Git for AI agents. The platform provides Linux microVMs that boot in under 600ms with live-fork, pause-resume, and persistent snapshots; a multi-tenant Git service with branchable filesystems, GitHub Sync, full-text search, and webhook triggers; an Execute (Serverless Runs) API for ephemeral JavaScript/TypeScript code; a Web Deployments API for hosted Node.js apps and static sites; Cron schedules; custom Domains with wildcard SSL; an Identity service for scoped per-user and per-agent access tokens; and Observability logs. Freestyle is a direct sandbox option for AI app builders, background agents, code review bots, and long-running assistants — a usage-priced alternative to running Anthropic's hosted Code Execution tool or building bespoke microVM infrastructure on Firecracker, Modal, or E2B.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/freestyle-sh/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/freestyle-sh/refs/heads/main/apis.yml)

## Scope

- **Position:** Producing
- **Access:** 3rd-Party

## Tags

- AI
- Agents
- Sandboxes
- VMs
- MicroVMs
- Git
- Code Execution
- JavaScript
- TypeScript
- Serverless
- Hosting
- Developer Tools
- Infrastructure

## Timestamps

- **Created:** 2026-05-25T00:00:00.000Z
- **Modified:** 2026-05-25

## APIs

### Freestyle VMs API

Create, snapshot, fork, suspend, resume, exec, and manage Linux microVMs designed for AI agents. VMs boot in under 600ms with restored memory snapshots, support live-forking a running VM into multiple copies in milliseconds, and can be paused after idle to $0 cost and resumed on next exec. Includes systemd service management, terminal logs/xterm-256color streams, file get/put/watch, and stats streaming.

- **Human URL:** [https://docs.freestyle.sh/v2/vms/about](https://docs.freestyle.sh/v2/vms/about)

#### Tags

- Agents
- AI
- Sandboxes
- VMs
- MicroVMs
- Code Execution

#### Properties

- [Documentation](https://docs.freestyle.sh/v2/vms/about)
- [Documentation](https://docs.freestyle.sh/v2/vms/lifecycle)
- [Documentation](https://docs.freestyle.sh/v2/vms/configuration)
- [Documentation](https://docs.freestyle.sh/v2/vms/templates-snapshots)
- [Documentation](https://docs.freestyle.sh/v2/vms/ssh-access)
- [OpenAPI](openapi/freestyle-vm-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/freestyle-vm-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/freestyle-vm-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/freestyle-vm-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON-LD](json-ld/freestyle-sh-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)

### Freestyle Git API

Multi-tenant hosted Git for AI agents — every agent gets a branchable filesystem with commits, diffs, rollback, and review. Includes create/list/delete repositories, commits from files or from raw Git objects, branches and tags, tree/blob inspection, full-text file/commit/diff search, repository compare, tarball/zip downloads, GitHub bidirectional sync, repair jobs, and webhook triggers.

- **Human URL:** [https://docs.freestyle.sh/v2/git/about](https://docs.freestyle.sh/v2/git/about)

#### Tags

- Git
- Agents
- AI
- Version Control
- Multi-tenant

#### Properties

- [Documentation](https://docs.freestyle.sh/v2/git/about)
- [Documentation](https://docs.freestyle.sh/v2/git/repos)
- [Documentation](https://docs.freestyle.sh/v2/git/search)
- [Documentation](https://docs.freestyle.sh/v2/git/hooks)
- [Documentation](https://docs.freestyle.sh/v2/git/github-sync)
- [Documentation](https://docs.freestyle.sh/v2/git/advanced/database-api)
- [OpenAPI](openapi/freestyle-git-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/freestyle-git-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/freestyle-git-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/freestyle-repository-schema.json) — [JSON Schema](https://json-schema.org/specification)

### Freestyle Identity API

Identity and access management for end users and AI agents. Create identities, mint and revoke access tokens, grant per-repo Git permissions (read/write/admin), grant per-VM permissions with an allowed-users list, and inspect the current bearer-token whoami plus long-running background-request status.

- **Human URL:** [https://docs.freestyle.sh/v2/about](https://docs.freestyle.sh/v2/about)

#### Tags

- Identity
- Access Management
- Permissions
- Tokens
- Agents

#### Properties

- [Documentation](https://docs.freestyle.sh/v2/about)
- [OpenAPI](openapi/freestyle-identity-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/freestyle-identity-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/freestyle-identity-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON-LD](json-ld/freestyle-sh-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)

### Freestyle Domains API

Manage custom domains for Freestyle Web Deployments and VMs — list domains, create/verify ownership, insert and remove domain → deployment mappings, provision wildcard SSL certificates, and manage DNS records for Freestyle-hosted domains.

- **Human URL:** [https://docs.freestyle.sh/v2/domains](https://docs.freestyle.sh/v2/domains)

#### Tags

- Domains
- DNS
- Certificates
- SSL

#### Properties

- [Documentation](https://docs.freestyle.sh/v2/domains)
- [Documentation](https://docs.freestyle.sh/v2/domains/deploy-to-custom-domain)
- [OpenAPI](openapi/freestyle-domains-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/freestyle-domains-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/freestyle-domains-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Freestyle Execute API

Serverless Runs — execute JavaScript or TypeScript code on demand and get the result. No deployment, no HTTP server — POST code and receive the output. Supports node modules, environment variables, egress control, and stored run output retrieval. The v3 endpoint is the current execute surface; v1 is deprecated.

- **Human URL:** [https://docs.freestyle.sh/v2/serverless/runs/about](https://docs.freestyle.sh/v2/serverless/runs/about)

#### Tags

- Code Execution
- JavaScript
- TypeScript
- Sandboxes
- Agents
- AI

#### Properties

- [Documentation](https://docs.freestyle.sh/v2/serverless/runs/about)
- [Documentation](https://docs.freestyle.sh/v2/serverless/runs/code-playground)
- [Documentation](https://docs.freestyle.sh/v2/serverless/runs/egress)
- [Documentation](https://docs.freestyle.sh/v2/serverless/runs/errors)
- [OpenAPI](openapi/freestyle-execute-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/freestyle-execute-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/freestyle-execute-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Freestyle Web Deployments API

Deploy and manage Node.js web applications and static sites. Push code via /web/v1/deployment, list deployments, inspect deployment metadata, and fetch/update files on a deployment using HTTP-style verb-based operations. Handles node-module caching, scaling, wildcard subdomains, and SSL certificates end-to-end.

- **Human URL:** [https://docs.freestyle.sh/v2/serverless/deployments/about](https://docs.freestyle.sh/v2/serverless/deployments/about)

#### Tags

- Hosting
- Deployments
- Node.js
- JavaScript
- TypeScript

#### Properties

- [Documentation](https://docs.freestyle.sh/v2/serverless/deployments/about)
- [Documentation](https://docs.freestyle.sh/v2/serverless/deployments/configuration)
- [Documentation](https://docs.freestyle.sh/v2/serverless/deployments/cron-jobs)
- [Documentation](https://docs.freestyle.sh/v2/serverless/deployments/guides/nextjs)
- [Documentation](https://docs.freestyle.sh/v2/serverless/deployments/guides/vite)
- [Documentation](https://docs.freestyle.sh/v2/serverless/deployments/guides/static)
- [OpenAPI](openapi/freestyle-web-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/freestyle-web-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/freestyle-web-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Freestyle Cron API

Schedule recurring serverless runs. Create, update, and delete cron schedules; list past executions; inspect per-schedule success rate and a metrics timeline for observability.

- **Human URL:** [https://docs.freestyle.sh/v2/serverless/deployments/cron-jobs](https://docs.freestyle.sh/v2/serverless/deployments/cron-jobs)

#### Tags

- Cron
- Scheduling
- Serverless

#### Properties

- [Documentation](https://docs.freestyle.sh/v2/serverless/deployments/cron-jobs)
- [OpenAPI](openapi/freestyle-cron-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/freestyle-cron-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/freestyle-cron-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Freestyle Observability API

Query structured logs across Freestyle services. Filter by VM, deployment, run, identity, or time range to debug agent runs end-to-end.

- **Human URL:** [https://docs.freestyle.sh/v2/about](https://docs.freestyle.sh/v2/about)

#### Tags

- Observability
- Logs
- Monitoring

#### Properties

- [Documentation](https://docs.freestyle.sh/v2/about)
- [OpenAPI](openapi/freestyle-observability-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/freestyle-observability-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/freestyle-observability-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [Portal](https://www.freestyle.sh)
- [Documentation](https://docs.freestyle.sh)
- [Documentation](https://docs.freestyle.sh/v2)
- [Getting Started](https://docs.freestyle.sh/v2/about)
- [OpenAPI](https://api.freestyle.sh/openapi.json) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Sign Up](https://admin.freestyle.sh)
- [Dashboard](https://admin.freestyle.sh)
- [Pricing](https://www.freestyle.sh/pricing)
- [Blog](https://www.freestyle.sh/blog)
- [Status Page](https://status.freestyle.sh)
- [Forum](https://discord.com/invite/YTRprVkdnz)
- [Privacy Policy](https://www.freestyle.sh/privacy)
- [GitHub Organization](https://github.com/freestyle-sh)
- [SDK](https://github.com/freestyle-sh/sandbox_sdks)
- [SDK](https://github.com/freestyle-sh/sandbox-sdks-py)
- [SDK](https://github.com/freestyle-sh/rigkit)
- [Tool](https://github.com/freestyle-sh/freestyle-auth)
- [Tool](https://github.com/freestyle-sh/Adorable)
- [Tool](https://github.com/freestyle-sh/cloudstate)
- [Code Examples](https://github.com/freestyle-sh/freestyle-execute-chat)
- [Code Examples](https://github.com/freestyle-sh/freestyle-astro-template)
- [Code Examples](https://github.com/freestyle-sh/freestyle-sveltekit-template)
- [Code Examples](https://github.com/freestyle-sh/freestyle-solid-template)
- [Code Examples](https://github.com/freestyle-sh/freestyle-next-template)
- [Code Examples](https://github.com/freestyle-sh/freestyle-vite-react)
- [Code Examples](https://github.com/freestyle-sh/freestyle-react-native-template)
- [Code Examples](https://github.com/freestyle-sh/freestyle-deno-template)
- [Code Examples](https://github.com/freestyle-sh/freestyle-expo)
- [Documentation](https://docs.freestyle.sh/v2/vms/integrations/node)
- [Documentation](https://docs.freestyle.sh/v2/vms/integrations/python)
- [Documentation](https://docs.freestyle.sh/v2/vms/integrations/bun)
- [Documentation](https://docs.freestyle.sh/v2/vms/integrations/deno)
- [Documentation](https://docs.freestyle.sh/v2/vms/integrations/ruby)
- [Documentation](https://docs.freestyle.sh/v2/vms/integrations/java)
- [Documentation](https://docs.freestyle.sh/v2/vms/integrations/postgres)
- [Documentation](https://docs.freestyle.sh/v2/vms/integrations/opencode)
- [Documentation](https://docs.freestyle.sh/v2/vms/integrations/web-terminal)
- [Documentation](https://docs.freestyle.sh/v2/vms/custom-integrations)
- [Documentation](https://docs.freestyle.sh/v2/vms/cli)
- [Documentation](https://docs.freestyle.sh/v2/git/cli)
- [Documentation](https://docs.freestyle.sh/v2/serverless/deployments/cli)
- [Documentation](https://docs.freestyle.sh/v2/serverless/runs/cli)
- [Documentation](https://docs.freestyle.sh/v2/domains/cli)
- [Plans](plans/freestyle-sh-plans-pricing.yml)
- [Rate Limits](rate-limits/freestyle-sh-rate-limits.yml)
- [Fin Ops](finops/freestyle-sh-finops.yml)
- [Features](undefined)
- [Use Cases](undefined)
- [Integrations](undefined)
- [Solutions](undefined)

## Maintainers

**FN:** Kin Lane
**Email:** info@apievangelist.com
**URL:** https://apievangelist.com
