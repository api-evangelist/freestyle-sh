# Freestyle (freestyle-sh)

Freestyle is the infrastructure for code you didn't write — VMs and Git for AI agents. The platform provides Linux microVMs that boot in under 600ms with live-fork, pause-resume, and persistent snapshots; a multi-tenant Git service with branchable filesystems, GitHub Sync, full-text search, and webhook triggers; an Execute (Serverless Runs) API for ephemeral JavaScript/TypeScript code; a Web Deployments API for hosted Node.js apps and static sites; Cron schedules; custom Domains with wildcard SSL; an Identity service for scoped per-user and per-agent access tokens; and Observability logs. Freestyle is a direct sandbox option for AI app builders, background agents, code review bots, and long-running assistants — a usage-priced alternative to running Anthropic's hosted Code Execution tool or building bespoke microVM infrastructure on Firecracker, Modal, or E2B.

**URL:** [Visit APIs.json](https://raw.githubusercontent.com/api-evangelist/freestyle-sh/refs/heads/main/apis.yml)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags

 - AI, Agents, Sandboxes, VMs, MicroVMs, Git, Code Execution, JavaScript, TypeScript, Serverless, Hosting, Developer Tools, Infrastructure

## Timestamps

- **Created:** 2026-05-25
- **Modified:** 2026-05-25

## Plans

| Plan | Price | Concurrent VMs | Managed Domains | Repositories | Runs/Month |
|---|---|---|---|---|---|
| Free | $0 forever | 10 | 5 | 500 | 500 |
| Hobby | $50/mo + usage over $50 | 40 | 20 | 5,000 | 5,000 |
| Pro | $500/mo + usage over $500 | 400 | 2,000 | 50,000 | 500,000 |
| Enterprise | Custom | Custom | Custom | Custom | Custom |

## VM Usage Pricing

| Resource | Price | Free Tier Daily Allowance |
|---|---|---|
| vCPU-hour | $0.04032 | 20 |
| GiB-memory-hour | $0.0129 | 40 |
| GiB-storage-hour | $0.000086 | 16,800 |

Persistent Snapshots, Persistent VMs, and Custom Sizing require Hobby or higher. Pro caps each VM at 32 vCPUs, 32 GB memory, and 64 GB disk.

## APIs

### Freestyle VMs API
Create, snapshot, fork, suspend, resume, exec, and manage Linux microVMs designed for AI agents. VMs boot in under 600ms with restored memory snapshots, support live-forking a running VM into multiple copies in milliseconds, and can be paused after idle to $0 cost. Includes systemd service management, terminal logs/xterm-256color streams, file get/put/watch, and stats streaming.

**Human URL:** [https://docs.freestyle.sh/v2/vms/about](https://docs.freestyle.sh/v2/vms/about)

- [Documentation — About](https://docs.freestyle.sh/v2/vms/about)
- [Documentation — Lifecycle](https://docs.freestyle.sh/v2/vms/lifecycle)
- [Documentation — Configuration](https://docs.freestyle.sh/v2/vms/configuration)
- [Documentation — Templates and Snapshots](https://docs.freestyle.sh/v2/vms/templates-snapshots)
- [Documentation — SSH Access](https://docs.freestyle.sh/v2/vms/ssh-access)
- [OpenAPI](openapi/freestyle-vm-api-openapi.yml)
- [JSON Schema — VM](json-schema/freestyle-vm-schema.json)
- [JSON-LD](json-ld/freestyle-sh-context.jsonld)
- [Naftiko Capability — VMs](capabilities/vm-vms.yaml)
- [Naftiko Capability — Snapshots](capabilities/vm-snapshots.yaml)
- [Naftiko Capability — Builds](capabilities/vm-builds.yaml)
- [Naftiko Capability — Files](capabilities/vm-files.yaml)
- [Naftiko Capability — Systemd](capabilities/vm-systemd.yaml)
- [Naftiko Capability — Terminals](capabilities/vm-terminals.yaml)

### Freestyle Git API
Multi-tenant hosted Git for AI agents — every agent gets a branchable filesystem with commits, diffs, rollback, and review. Includes create/list/delete repositories, commits from files or from raw Git objects, branches and tags, tree/blob inspection, full-text file/commit/diff search, repository compare, tarball/zip downloads, GitHub bidirectional sync, repair jobs, and webhook triggers.

**Human URL:** [https://docs.freestyle.sh/v2/git/about](https://docs.freestyle.sh/v2/git/about)

- [Documentation — About](https://docs.freestyle.sh/v2/git/about)
- [Documentation — Manage Repositories](https://docs.freestyle.sh/v2/git/repos)
- [Documentation — Search](https://docs.freestyle.sh/v2/git/search)
- [Documentation — Triggers and Webhooks](https://docs.freestyle.sh/v2/git/hooks)
- [Documentation — GitHub Sync](https://docs.freestyle.sh/v2/git/github-sync)
- [Documentation — Advanced Database API](https://docs.freestyle.sh/v2/git/advanced/database-api)
- [OpenAPI](openapi/freestyle-git-api-openapi.yml)
- [JSON Schema — Repository](json-schema/freestyle-repository-schema.json)
- [Naftiko Capability — Repo](capabilities/git-repo.yaml)
- [Naftiko Capability — Commits](capabilities/git-commits.yaml)
- [Naftiko Capability — Branches](capabilities/git-branches.yaml)
- [Naftiko Capability — Tags](capabilities/git-tags.yaml)
- [Naftiko Capability — Trees](capabilities/git-trees.yaml)
- [Naftiko Capability — Blobs](capabilities/git-blobs.yaml)
- [Naftiko Capability — Search](capabilities/git-search.yaml)
- [Naftiko Capability — Triggers](capabilities/git-triggers.yaml)
- [Naftiko Capability — GitHub Sync](capabilities/git-github-sync.yaml)
- [Naftiko Capability — Repair](capabilities/git-repair.yaml)

### Freestyle Identity API
Identity and access management for end users and AI agents. Create identities, mint and revoke access tokens, grant per-repo Git permissions (read/write/admin), grant per-VM permissions with an allowed-users list, and inspect the current bearer-token whoami plus long-running background-request status.

**Human URL:** [https://docs.freestyle.sh/v2/about](https://docs.freestyle.sh/v2/about)

- [OpenAPI](openapi/freestyle-identity-api-openapi.yml)
- [JSON-LD](json-ld/freestyle-sh-context.jsonld)
- [Naftiko Capability — Identities](capabilities/identity-identities.yaml)
- [Naftiko Capability — Tokens](capabilities/identity-tokens.yaml)
- [Naftiko Capability — Git Permissions](capabilities/identity-git-permissions.yaml)
- [Naftiko Capability — VM Permissions](capabilities/identity-vm-permissions.yaml)
- [Naftiko Capability — Auth](capabilities/identity-auth.yaml)

### Freestyle Domains API
Manage custom domains for Freestyle Web Deployments and VMs — list domains, create/verify ownership, insert and remove domain → deployment mappings, provision wildcard SSL certificates, and manage DNS records for Freestyle-hosted domains.

**Human URL:** [https://docs.freestyle.sh/v2/domains](https://docs.freestyle.sh/v2/domains)

- [Documentation — Verify your domain](https://docs.freestyle.sh/v2/domains)
- [Documentation — Deploy to Custom Domain](https://docs.freestyle.sh/v2/domains/deploy-to-custom-domain)
- [OpenAPI](openapi/freestyle-domains-api-openapi.yml)
- [Naftiko Capability — Domains](capabilities/domains-domains.yaml)
- [Naftiko Capability — Verifications](capabilities/domains-verifications.yaml)
- [Naftiko Capability — Mappings](capabilities/domains-mappings.yaml)
- [Naftiko Capability — Certificates](capabilities/domains-certs.yaml)
- [Naftiko Capability — DNS Records](capabilities/domains-dns-records.yaml)

### Freestyle Execute API
Serverless Runs — execute JavaScript or TypeScript code on demand and get the result. No deployment, no HTTP server — POST code and receive the output. Supports node modules, environment variables, egress control, and stored run output retrieval. The v3 endpoint is the current execute surface; v1 is deprecated.

**Human URL:** [https://docs.freestyle.sh/v2/serverless/runs/about](https://docs.freestyle.sh/v2/serverless/runs/about)

- [Documentation — About](https://docs.freestyle.sh/v2/serverless/runs/about)
- [Documentation — Code Playground](https://docs.freestyle.sh/v2/serverless/runs/code-playground)
- [Documentation — Egress Control](https://docs.freestyle.sh/v2/serverless/runs/egress)
- [Documentation — Errors](https://docs.freestyle.sh/v2/serverless/runs/errors)
- [OpenAPI](openapi/freestyle-execute-api-openapi.yml)
- [Naftiko Capability — Execute](capabilities/execute-execute.yaml)

### Freestyle Web Deployments API
Deploy and manage Node.js web applications and static sites. Push code via /web/v1/deployment, list deployments, inspect deployment metadata, and fetch/update files on a deployment using HTTP-style verb-based operations. Handles node-module caching, scaling, wildcard subdomains, and SSL certificates end-to-end.

**Human URL:** [https://docs.freestyle.sh/v2/serverless/deployments/about](https://docs.freestyle.sh/v2/serverless/deployments/about)

- [Documentation — About](https://docs.freestyle.sh/v2/serverless/deployments/about)
- [Documentation — Configuration](https://docs.freestyle.sh/v2/serverless/deployments/configuration)
- [Documentation — Cron Jobs](https://docs.freestyle.sh/v2/serverless/deployments/cron-jobs)
- [Guide — Next.js](https://docs.freestyle.sh/v2/serverless/deployments/guides/nextjs)
- [Guide — Vite](https://docs.freestyle.sh/v2/serverless/deployments/guides/vite)
- [Guide — Static Hosting](https://docs.freestyle.sh/v2/serverless/deployments/guides/static)
- [OpenAPI](openapi/freestyle-web-api-openapi.yml)
- [Naftiko Capability — Deployments](capabilities/web-deployments.yaml)

### Freestyle Cron API
Schedule recurring serverless runs. Create, update, and delete cron schedules; list past executions; inspect per-schedule success rate and a metrics timeline for observability.

**Human URL:** [https://docs.freestyle.sh/v2/serverless/deployments/cron-jobs](https://docs.freestyle.sh/v2/serverless/deployments/cron-jobs)

- [OpenAPI](openapi/freestyle-cron-api-openapi.yml)
- [Naftiko Capability — Schedules](capabilities/cron-schedules.yaml)

### Freestyle Observability API
Query structured logs across Freestyle services. Filter by VM, deployment, run, identity, or time range to debug agent runs end-to-end.

**Human URL:** [https://docs.freestyle.sh/v2/about](https://docs.freestyle.sh/v2/about)

- [OpenAPI](openapi/freestyle-observability-api-openapi.yml)
- [Naftiko Capability — Logs](capabilities/observability-logs.yaml)

## Common Properties

- [Portal](https://www.freestyle.sh)
- [Documentation](https://docs.freestyle.sh)
- [Getting Started](https://docs.freestyle.sh/v2/about)
- [OpenAPI (full)](https://api.freestyle.sh/openapi.json)
- [Pricing](https://www.freestyle.sh/pricing)
- [Blog](https://www.freestyle.sh/blog)
- [Status](https://status.freestyle.sh)
- [Discord](https://discord.com/invite/YTRprVkdnz)
- [Dashboard / Sign Up](https://admin.freestyle.sh)
- [Privacy Policy](https://www.freestyle.sh/privacy)
- [GitHub Organization](https://github.com/freestyle-sh)
- [TypeScript SDK — sandbox_sdks](https://github.com/freestyle-sh/sandbox_sdks)
- [Python SDK — sandbox-sdks-py](https://github.com/freestyle-sh/sandbox-sdks-py)
- [CLI/SDK — rigkit](https://github.com/freestyle-sh/rigkit)
- [Adorable — Open Source Lovable](https://github.com/freestyle-sh/Adorable)
- [Cloudstate — JavaScript Database](https://github.com/freestyle-sh/cloudstate)
- [Freestyle Auth](https://github.com/freestyle-sh/freestyle-auth)
- [Plans](plans/freestyle-sh-plans-pricing.yml)
- [Rate Limits](rate-limits/freestyle-sh-rate-limits.yml)
- [FinOps](finops/freestyle-sh-finops.yml)

## VM Language Integrations

Node.js · Bun · Deno · Python (with uv) · Ruby · Java · PostgreSQL · OpenCode · Web Terminal · Custom integrations

## Use Cases

- AI app builders (Lovable, Bolt, V0 style) provisioning a sandbox VM per project with cloned source, dev servers, and `*.style.dev` preview domains
- Background agents (Devin, Cursor Agent style) forking a base VM into parallel workers — one builds the API, one builds the UI, one writes tests
- Code review bots (CodeRabbit, Greptile style) cloning a repo at a PR SHA, running lint/test, and posting a Claude-generated review
- Long-running AI assistants (Claude, OpenClaw, Cowork style) using a persistent VM with 60s idle pause to keep per-user state at $0 cost between turns
- LLM code-interpreter style — execute model-generated code safely in an isolated microVM with egress control
- Sandboxed AI agent evals on ephemeral microVMs (one VM per eval run)
- Hosted code playgrounds for educational and developer-tool products

## Maintainers

| Name | Email | URL |
|---|---|---|
| Kin Lane | info@apievangelist.com | [https://apievangelist.com](https://apievangelist.com) |
