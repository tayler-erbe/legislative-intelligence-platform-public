# Handoff: where the work is and how to continue

Updated 24 November 2026. This public repository is the scrubbed showcase, frozen at the 5 November source release. **Active work, stakeholder details and meeting preparation are in the private repository**, which is not public. This file only points to them, and holds no names, addresses or resource details.

## Where things are

| What | Where |
|---|---|
| Public showcase (this repo) | Architecture, scrubbed source, runbook: [SYSTEM_GUIDE.md](SYSTEM_GUIDE.md), [OPERATIONS.md](OPERATIONS.md), [knowledge-index.json](knowledge-index.json) |
| Private working repo | `tayler-erbe/legislative-intelligence-platform-private` |
| Start-here file (private) | `docs/HANDOFF.md`: read the 24 November update at the top |
| Every change since QA, with test steps (private) | `docs/QA_CHANGELOG.md` |
| Stakeholder meeting brief (private, restricted) | `docs/restricted/` (listed in its README) |
| Stakeholders, requests, outreach (private, restricted) | `docs/restricted/STAKEHOLDER_TRACKER.md` |

## Private repository branches

| Branch | Meaning |
|---|---|
| `frozen/qa-passed-2026-11-05` | The build that passed QA. Do not change it. |
| `frozen/pre-build-2026-11-19` | Post-QA work frozen before new building. Do not change it. |
| `claude/peaceful-newton-u9rfmg` | Current work |

## Status in one paragraph

The platform passed QA on 5 November. Since then these have been built, but none of them is deployed:
- hearing alerts
- a pipeline health alert
- relevance feedback
- the extraction v2 tooling
- a fix so failed sign-in emails are reported instead of hidden
- an offline tool that builds per-bill dossiers from exported email

A live issue is open: sign-in emails have not arrived since a Microsoft service outage in mid-November. The diagnosis steps are in the private handoff.

## Rules for whoever continues

Keep this public repo free of the following:
- stakeholder names
- email addresses
- Azure resource names
- user data
- credentials

Those stay in the private repo, under `docs/restricted/`.

Distinguish built and tested offline from deployed and working. See the public [AGENTS.md](../AGENTS.md) and the private repo's `AGENTS.md`.
