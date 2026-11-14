# Free n8n starter workflows

Three minimal, importable n8n workflows to get a self-hosted instance doing something useful in
five minutes. Copy the JSON, paste it into n8n (**Workflows → Import from clipboard**), connect
your credentials, run.

| File | What it does | Nodes |
|---|---|---|
| `workflows/01-webhook-to-http.json` | Public webhook that calls any JSON API and returns the response | Webhook → HTTP Request |
| `workflows/02-rss-digest.json` | Pulls an RSS feed and keeps only the newest N items | RSS Read → Limit |
| `workflows/03-schedule-to-api.json` | Every 6 hours, call an API and keep the result | Schedule → HTTP Request |

## Import

1. Open n8n → **Workflows** → **Import from clipboard**.
2. Paste the contents of a file from `workflows/`.
3. Open the HTTP Request node and set your URL (or keep the example).
4. Activate the workflow.

## Why these are free

They are the smallest possible building blocks — the wiring, not the business logic. The parts that
usually take days (lead capture with AI scoring, enrichment, client onboarding sequences, error
handling, retries) are packaged as tested, documented packs at
**[workflowpacks.com](https://workflowpacks.com/)**.

- [Lead Gen Pack](https://workflowpacks.com/lead-gen-pack/) — capture, enrich and score inbound leads
- [Client Ops Pack](https://workflowpacks.com/client-ops-pack/) — onboarding and follow-up sequences
- [Content Repurposing Pack](https://workflowpacks.com/content-repurposing-pack/) — one input, many formats

Comparing tools before you commit? [n8n vs Zapier (2026), with real prices](https://workflowpacks.com/blog/n8n-vs-zapier/).

## Notes

- Tested against n8n 1.x. Node type versions in the JSON may upgrade automatically on import.
- No credentials are included. Nothing here phones home.
- License: MIT for these templates. n8n itself is fair-code; see the n8n repository.
