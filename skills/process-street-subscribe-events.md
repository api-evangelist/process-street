---
name: Subscribe to Process Street events with a webhook
description: Register an outgoing webhook for task and workflow-run events and manage the subscription.
api: openapi/process-street-openapi-original.json
operations:
- createWebhook
- listWebhooks
- getWebhook
- updateWebhook
- deleteWebhook
---

# Subscribe to Process Street events with a webhook

Get notified when tasks and workflow runs change by registering an **outgoing webhook**.

## Auth
`X-API-KEY: <your-key>`. Base URL `https://public-api.process.st/api/v1.1`.

## Steps
1. **Create the subscription.** `createWebhook` with a target `url` and a set of `triggers`. Valid triggers: `TaskChecked`, `TaskUnchecked`, `TaskCheckedUnchecked`, `TaskReady`, `WorkflowRunCreated`, `WorkflowRunCompleted`.
2. **Verify.** `listWebhooks` / `getWebhook` to confirm the subscription and its `status`.
3. **Maintain.** `updateWebhook` to change the URL or triggers; `deleteWebhook` to remove it (idempotent — deleting an already-deleted webhook returns `404`, safe to ignore).

## Notes
- For inbound automation (external systems starting runs or writing data sets) use the incoming-webhook endpoints instead — see asyncapi/process-street-webhooks.yml.
- Honor `Retry-After` on `429`; branch on `errorCode`.
