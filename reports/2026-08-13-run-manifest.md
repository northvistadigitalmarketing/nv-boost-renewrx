# NVM Boost Run Manifest — 2026-08-13

- **Contract:** NV-2026-RNWRX (Marketing Services Agreement, RenewRX)
- **Doc Ref:** DFB338CA-537D-4A8A-BA7E-F6B05B9F949C
- **Client slug:** renewrx · **Repo:** northvistadigitalmarketing/nv-boost-renewrx (public)
- **Live URL:** https://northvistadigitalmarketing.github.io/nv-boost-renewrx/ (placeholder, noindex — provisioning only, not a marketing deliverable)
- **Mode:** AUTO-RUN, no full-auto pre-grant given — all three hard gates (ad spend, live-campaign changes, real-client publishing) remain unresolved and untouched this run.

## Phase 0 — Provision

| Step | Result |
|---|---|
| Get Repository | Not found — proceeded to create |
| Create from Template (North_Vista_Digital_Marketing) | Success — repo ID 1333467219, public |
| Provisioning commit (README, client-profile, docs/index.html — sanitized) | Success — commit c5de27e144354b8e2961854dd1572de5fd143db9 |
| Enable Pages (main, /docs) | Success |
| Pages build verification | run 31735703804 — completed / success |

## Step 1 — Contract intake filing (RESOLVED 2026-08-13, later same day)

- Blocked earlier this run (no device folder connected to stage the PDF to the local machine running Krista's upload tool).
- User connected folder `/Users/taylortabile/Krista Test`; PDF staged there, then `krista_upload_file` → `krista_skill_nv-contract-intake-filer` → `krista_skill_krista-docset-filer`.
- **Docset override:** requested `nv-boost-renewrx`, filed to `north-vista-marketing` per the filer's v0.3.0 single-doc-set policy (2026-08-13 direction, N. Grant) — all North Vista filings now land in one agency-wide doc set.
- Add Document conversation `CEC_auto_e41110dd-5fbc-4266-b0ca-6d3347dc4208` — completed. Two benign `fromIndex = -1` submit errors during PDF indexing (documented behavior — status polled instead of blind-retrying).
- Read-back verified via `answer_question(north-vista-marketing, …)` — correctly cited `NVM_Contract_RenewRX_07292026.pdf` with fee/term/effective-date detail.
- Logged to Delivery Log (client-profile.md) in the same-day filing commit.

## Deliverables spec (Scope of Work → resolution)

| ID | Contract line | Class | Tier | Resolution | Decision | Blocker |
|---|---|---|---|---|---|---|
| D1 | CRM Workspace | ongoing_service | conversation (GoHighLevel) | No 1:1 conversation/skill found in current catalog for initial CRM setup | hold | needs build — flag to Onboarding Agent or new conversation |
| D2 | Live reporting dashboard | ongoing_service | conversation | No resolved conversation/skill for dashboard provisioning | hold | needs build |
| D3 | Google Business Profile optimization | ongoing_service (monthly) | client-skill → gbp-optimizer (APPROVED) | Recurring cadence not yet Krista-scheduled | hold (substitute: client-side-schedule flagged) | needs scheduling decision; gbp-optimizer is name-gated, not run this turn |
| D4 | Paid Google search ads | ongoing_service + spend | client-skill → google-search-campaign-builder (spec only) / Google Ads invoker (live) | Spec-build not yet run; launch is hard-gated | hold | **hard gate: ad spend / live campaign — needs explicit approval, never pre-granted** |
| D5 | Paid Meta ads | ongoing_service + spend | client-skill → meta-ad-copy (spec only) / META invoker (live) | Spec-build not yet run; launch is hard-gated | hold | **hard gate: ad spend / live campaign — needs explicit approval** |
| D6 | Conversion landing page | artifact | client-skill → local-landing-page-builder | Draft not yet built | hold | build is fine; publishing to docs/ is **hard gate: real-client publishing — needs explicit approval** |
| D7 | Call tracking for lead attribution | ongoing_service | conversation (GoHighLevel) | No resolved conversation/skill found | hold | needs build |

## Backlog (build gaps)

- D1, D2, D7 have no resolved Krista conversation in the current agent/skill catalog for initial setup — flagged for a follow-up build (likely under the GoHighLevel Business Automation Agent or Onboarding Agent, both currently low/no conversation history).
- D3 recurring cadence needs a Krista-native schedule once gbp-optimizer is explicitly invoked for this client.

## Hard gates — untouched this run (require explicit per-item approval)

1. Real ad spend / campaign creation (Google Ads, Meta) — D4, D5.
2. Changes to a live campaign — n/a yet (no campaign exists).
3. Client-facing publishing for RenewRX (a real, non-demo client) — D6 landing page, and any future docs/ content beyond the noindex placeholder.

None of the above were pre-approved in this run's invocation, so none were executed, per policy.

## Open items for Taylor

- Confirm whether to proceed with drafting (not publishing) the landing page (D6) and ad copy (D4/D5) now — these are draft-only and don't touch spend or go live.
- Decide who/what resolves the CRM Workspace, dashboard, and call-tracking setup (D1, D2, D7) — no existing Krista conversation matched cleanly.
