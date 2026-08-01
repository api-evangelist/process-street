---
name: Complete tasks and fill form fields on a workflow run
description: Walk a running workflow run's tasks, fill in form field values, assign, and mark tasks complete.
api: openapi/process-street-openapi-original.json
operations:
- getWorkflowRun
- listTasks
- assignTask
- batchUpdateFormFieldValues
- updateTask
---

# Complete tasks and fill form fields on a workflow run

Advance an in-progress **workflow run** by filling form fields and completing tasks.

## Auth
`X-API-KEY: <your-key>`. Base URL `https://public-api.process.st/api/v1.1`.

## Steps
1. **Load the run.** `getWorkflowRun` for the run id.
2. **List its tasks.** `listTasks` (page with the `_` cursor / `next` link).
3. **Assign a task** (optional). `assignTask` to route work to a user.
4. **Fill form fields.** `batchUpdateFormFieldValues` to set multiple field values on a task in one idempotent call. Read current values first with `listFormFieldValues` if needed.
5. **Complete the task.** `updateTask` to set the task's completion status.

## Rules
- `PUT`/update calls are idempotent — safe to retry on `5xx`.
- Timestamps are ISO-8601 UTC with millisecond precision; date-only fields use a calendar date.
- Honor `Retry-After` on `429`; branch on `errorCode`.
