# Process Street

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

Process Street is a no-code workflow and process management platform for building, running, and automating recurring team processes as workflows (reusable templates) and workflow runs (checklists). Its REST Public API is organized around resource-oriented URLs, accepts and returns JSON, and covers workflows, workflow runs, tasks, form fields and values, pages, folders, data sets, users, one-off tasks, scheduled workflows, comments, attachments, outgoing webhooks, and incoming (data set + workflow) webhooks. Authentication is via an X-API-KEY header; results paginate through an opaque cursor with HATEOAS next links; and a hosted Model Context Protocol (MCP) server exposes most endpoints as tools for AI agents.

**Areas:** Company · Productivity · Workflows · Workflow Automation · Process Management · No-Code · Business Process · Task Management · Software-as-a-Service · MCP

## Process Street on APIs.io

Everything profiled for Process Street is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/process-street/](https://apis.io/providers/process-street/)** — or go straight to one of the APIs or properties below.

### APIs (28)

- [Process Street Attachments API](https://apis.io/apis/process-street/process-street-attachments-api/) — An attachment is a file uploaded to a task within a workflow run. Use these endpoints to list, upload, and delete task-level attachments.
- [Process Street Comments API](https://apis.io/apis/process-street/process-street-comments-api/) — A comment is a discussion message on a task within a workflow run. Use these endpoints to create, list, update, and delete comments.
- [Process Street Data Set Incoming Webhooks API](https://apis.io/apis/process-street/process-street-data-set-incoming-webhooks-api/) — An incoming webhook triggers data set row creation or updates from external systems. Use these endpoints to create, view, update, and delete incoming…
- [Process Street File Uploads API](https://apis.io/apis/process-street/process-street-file-uploads-api/) — A file upload is a two-step upload for large files. Create one to get an upload URL and a `fileUploadId`, send the file's bytes to that URL, then attach the…
- [Process Street Folders API](https://apis.io/apis/process-street/process-street-folders-api/) — A folder organizes workflows, pages, and other templates within your organization. Use these endpoints to create and manage folders.
- [Process Street Form Field Values API](https://apis.io/apis/process-street/process-street-form-field-values-api/) — A form field value is the data entered into a form field within a workflow run. Use these endpoints to read and update form field values for a specific…
- [Process Street Form Fields API](https://apis.io/apis/process-street/process-street-form-fields-api/) — A form field is a data-collection element defined on a workflow template. Use these endpoints to inspect the form fields and their available options on a…
- [Process Street My Work API](https://apis.io/apis/process-street/process-street-my-work-api/) — My Work is your personal task inbox — a consolidated view of all tasks and checklist items assigned to you across all workflows. Use these endpoints to…
- [Process Street One-Off Tasks API](https://apis.io/apis/process-street/process-street-one-off-tasks-api/) — A one-off task is a standalone task that can optionally be linked to a workflow run. Use these endpoints to create, view, and manage one-off tasks.
- [Process Street Page Revisions API](https://apis.io/apis/process-street/process-street-page-revisions-api/) — A page revision is a versioned snapshot of a page's content. Use these endpoints to list, inspect, and manage revisions.
- [Process Street Page Widgets API](https://apis.io/apis/process-street/process-street-page-widgets-api/) — A page widget is a content element (text, image, video, file, embed, cross-link, or table) on a page revision. Use these endpoints to create and manage…
- [Process Street Pages API](https://apis.io/apis/process-street/process-street-pages-api/) — A page is a document template for sharing information. Use these endpoints to create and manage pages.
- [Process Street Scheduled Workflows API](https://apis.io/apis/process-street/process-street-scheduled-workflows-api/) — A scheduled workflow is a recurring schedule that automatically creates workflow runs. Use these endpoints to list scheduled workflows and their recurrence…
- [Process Street Tasks API](https://apis.io/apis/process-street/process-street-tasks-api/) — A task is a step within a workflow run. Tasks can be checked off, assigned to users, and may contain form fields for collecting data. Use these endpoints to…
- [Process Street Users API](https://apis.io/apis/process-street/process-street-users-api/) — These endpoints let you list the users in your organization.
- [Process Street Utilities API](https://apis.io/apis/process-street/process-street-utilities-api/) — Helper endpoints for testing authentication and checking rate limits.
- [Process Street Webhooks API](https://apis.io/apis/process-street/process-street-webhooks-api/) — A webhook delivers real-time notifications to your application when events occur in Process Street. Use these endpoints to create and manage webhook…
- [Process Street Workflow Due Date Rules API](https://apis.io/apis/process-street/process-street-workflow-due-date-rules-api/) — A workflow due date rule defines how the checklist-level due date is calculated for workflow runs — either relative to the run's start date or derived from…
- [Process Street Workflow Incoming Webhooks API](https://apis.io/apis/process-street/process-street-workflow-incoming-webhooks-api/) — An incoming webhook triggers workflow runs from external systems. Use these endpoints to create, view, update, and delete incoming webhooks for a workflow.
- [Process Street Workflow Logic Rules API](https://apis.io/apis/process-street/process-street-workflow-logic-rules-api/) — Workflow logic rules are conditional rules that control the visibility of tasks and form fields within a workflow revision. Use these endpoints to create,…
- [Process Street Workflow Revisions API](https://apis.io/apis/process-street/process-street-workflow-revisions-api/) — A workflow revision is a versioned snapshot of a workflow's structure. Use these endpoints to list, inspect, and manage revisions.
- [Process Street Workflow Runs API](https://apis.io/apis/process-street/process-street-workflow-runs-api/) — A workflow run is an active instance of a workflow. Each run tracks its own progress, assignees, and form field values as it moves through the process. Use…
- [Process Street Workflow Task Assignment Rules API](https://apis.io/apis/process-street/process-street-workflow-task-assignment-rules-api/) — A workflow task assignment rule assigns a task template on a draft workflow revision to a specific user (static) or derives assignees from a source such as…
- [Process Street Workflow Task Due Date Rules API](https://apis.io/apis/process-street/process-street-workflow-task-due-date-rules-api/) — A task due date rule defines how an individual task's due date is calculated within a workflow run — relative to the run's start/due date, a form field…
- [Process Street Workflow Tasks API](https://apis.io/apis/process-street/process-street-workflow-tasks-api/) — A workflow task is a task template within a workflow revision. Use these endpoints to create, view, update, and delete task templates on draft revisions. >…
- [Process Street Workflow Widgets API](https://apis.io/apis/process-street/process-street-workflow-widgets-api/) — A workflow widget is a form field or content element on a task within a workflow revision. Use these endpoints to create and manage widgets on draft revisions.
- [Process Street Workflows API](https://apis.io/apis/process-street/process-street-workflows-api/) — A workflow is a reusable process template that defines the structure, tasks, and form fields for a repeatable process. Use these endpoints to browse and…
- [Process Street Datasets API](https://apis.io/apis/process-street/process-street-datasets-api/) — A data set is a structured collection of records that can be linked to workflow form fields. Use these endpoints to manage data sets and their records.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### AsyncAPI (1)

Event-driven and webhook contracts.

- [Process Street Webhooks](https://apis.io/asyncapis/process-street/process-street-webhooks/)

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [process-street](https://apis.io/servers/process-street/process-street/)

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Process Street Agentic Access](https://apis.io/agentic-access/process-street/process-street-agentic-access/)

#### Collections (28)

Postman and Open Collection request collections.

- [Process Street Public Attachments API](https://apis.io/collections/process-street/open-process-street-attachments-api/)
- [Process Street Public Attachments Comments API](https://apis.io/collections/process-street/open-process-street-comments-api/)
- [Process Street Public Attachments Data Set Incoming Webhooks API](https://apis.io/collections/process-street/open-process-street-data-set-incoming-webhooks-api/)
- [Process Street Public Attachments Data Sets API](https://apis.io/collections/process-street/open-process-street-data-sets-api/)
- [Process Street Public Attachments File Uploads API](https://apis.io/collections/process-street/open-process-street-file-uploads-api/)
- [Process Street Public Attachments Folders API](https://apis.io/collections/process-street/open-process-street-folders-api/)
- [Process Street Public Attachments Form Field Values API](https://apis.io/collections/process-street/open-process-street-form-field-values-api/)
- [Process Street Public Attachments Form Fields API](https://apis.io/collections/process-street/open-process-street-form-fields-api/)
- [Process Street Public Attachments My Work API](https://apis.io/collections/process-street/open-process-street-my-work-api/)
- [Process Street Public Attachments One-Off Tasks API](https://apis.io/collections/process-street/open-process-street-one-off-tasks-api/)
- [Process Street Public Attachments Page Revisions API](https://apis.io/collections/process-street/open-process-street-page-revisions-api/)
- [Process Street Public Attachments Page Widgets API](https://apis.io/collections/process-street/open-process-street-page-widgets-api/)
- [Process Street Public Attachments Pages API](https://apis.io/collections/process-street/open-process-street-pages-api/)
- [Process Street Public Attachments Scheduled Workflows API](https://apis.io/collections/process-street/open-process-street-scheduled-workflows-api/)
- [Process Street Public Attachments Tasks API](https://apis.io/collections/process-street/open-process-street-tasks-api/)
- [Process Street Public Attachments Users API](https://apis.io/collections/process-street/open-process-street-users-api/)
- [Process Street Public Attachments Utilities API](https://apis.io/collections/process-street/open-process-street-utilities-api/)
- [Process Street Public Attachments Webhooks API](https://apis.io/collections/process-street/open-process-street-webhooks-api/)
- [Process Street Public Attachments Workflow Due Date Rules API](https://apis.io/collections/process-street/open-process-street-workflow-due-date-rules-api/)
- [Process Street Public Attachments Workflow Incoming Webhooks API](https://apis.io/collections/process-street/open-process-street-workflow-incoming-webhooks-api/)
- [Process Street Public Attachments Workflow Logic Rules API](https://apis.io/collections/process-street/open-process-street-workflow-logic-rules-api/)
- [Process Street Public Attachments Workflow Revisions API](https://apis.io/collections/process-street/open-process-street-workflow-revisions-api/)
- [Process Street Public Attachments Workflow Runs API](https://apis.io/collections/process-street/open-process-street-workflow-runs-api/)
- [Process Street Public Attachments Workflow Task Assignment Rules API](https://apis.io/collections/process-street/open-process-street-workflow-task-assignment-rules-api/)
- [Process Street Public Attachments Workflow Task Due Date Rules API](https://apis.io/collections/process-street/open-process-street-workflow-task-due-date-rules-api/)
- …and 3 more published on APIs.io

#### Overlays (1)

OpenAPI overlays, including conversational phrasing for each operation.

- [Process Street Public Api Overlay](https://apis.io/overlays/process-street/process-street-public-api-overlay/)

#### Security (4)

Authentication, trust centre, and vulnerability disclosure.

- [Process Street Authentication](https://apis.io/security/process-street/process-street-authentication/)
- [Process Street Domain Security](https://apis.io/security/process-street/process-street-domain-security/)
- [Process Street Trust Center](https://apis.io/security/process-street/process-street-trust-center/)
- [Process Street Vulnerability Disclosure](https://apis.io/security/process-street/process-street-vulnerability-disclosure/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.process.st/)
- [Documentation](https://www.process.st/help/)
- [API reference](https://public-api.process.st/api/v1.1/docs/index.html)
- [Pricing](https://www.process.st/pricing/)
- [Sign up](https://app.process.st/organizations/create)
- [Support](https://www.process.st/help/)
- [Blog](https://www.process.st/blog/)
- [Security](https://www.process.st/responsible-disclosure/)
- [Compliance](https://www.process.st/security/)
- [Terms of service](https://www.process.st/terms-of-service/)
- [Privacy policy](https://www.process.st/privacy-policy/)
- [GitHub](https://github.com/process-street)
- [Status](https://status.process.st/)

## API Evangelist rating

**Kin Score 46.0** — developing · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 75.0 |
| Contract quality | 59.9 |
| Contract governance | 4.5 |
| Operational transparency | 36.8 |
| Developer ergonomics | 47.0 |
| Access clarity | 32.9 |

**Agent readiness 58.3** — agent-native

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | — |
| MCP Server | verified |
| Auth Clarity | served (partial credit) |
| Idempotency | documented (partial credit) |
| Error Semantics | documented (partial credit) |
| OpenAPI Examples | partial |
| Rate Limit Signal | — |
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
| Pagination Ratio | paginated |
| Operation Distinctiveness | distinct |

**Regulatory alignment 27.5** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/process-street/](https://apis.io/providers/process-street/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Process Street: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/process-street/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
