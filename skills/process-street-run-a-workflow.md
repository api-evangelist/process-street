---
name: Run a Process Street workflow
description: Find a workflow template and start a new workflow run (checklist) from it, idempotently.
api: openapi/process-street-openapi-original.json
operations:
- listWorkflows
- getWorkflow
- createWorkflowRun
- getWorkflowRun
---

# Run a Process Street workflow

Start one execution (a **workflow run**, aka checklist) of a reusable **workflow** template.

## Auth
Send `X-API-KEY: <your-key>` on every request. The key carries the permissions of the user who created it. Base URL: `https://public-api.process.st/api/v1.1`.

## Steps
1. **Find the template.** Call `listWorkflows` and pick the target workflow. Page with the `_` cursor: follow the `next` link in `links[]` until it is absent. Optionally call `getWorkflow` to inspect its tasks/form fields.
2. **Start a run idempotently.** Call `createWorkflowRun` with the workflow id and a stable `referenceId`. Because `POST` is not safe to blindly retry, the `referenceId` makes create idempotent — calling twice with the same `referenceId` returns the existing run instead of a duplicate.
3. **Read the live state.** Call `getWorkflowRun` to confirm the run and read its status.

## Rules
- IDs are opaque 22-char Muids — compare by string equality, never parse.
- On `429`, wait the `Retry-After` header duration before retrying.
- Branch error handling on `errorCode` (see errors/process-street-error-codes.yml), not the human `error` text.
