# Client Profile — RenewRX

> Read/written by Boost skills. Krista appends; humans read.

## Profile

- **Client:** RenewRX
- **Slug:** renewrx
- **Domain:** getrenewrx.com
- **Provisioned:** 2026-08-13
- **Active Lines:** Local Visibility (GBP & Lead Tracking), Paid Ads (Lead Generation)

## Agreement (sanitized — public repo)

- **Agreement No.:** NV-2026-RNWRX
- **Effective Date:** 2026-07-31 · **Initial Term:** 3 months, then month-to-month
- Full commercial terms (fee, billing, signatory contact info) are sealed in the signed MSA/SOW. Filed 2026-08-13 into the agency-wide Krista doc set `north-vista-marketing` (per the v0.3.0 single-doc-set policy — supersedes the per-client `nv-boost-renewrx` doc set named in earlier drafts of this profile); read-back verified. Not reproduced here.

## Business Summary

RenewRX (dba RenewRx) — https://getrenewrx.com/. Clinician-led hormone therapy, medical weight loss (GLP-1: semaglutide/tirzepatide), and peptide protocols. Single clinic at 6065 S. Highland Dr. Suite 1, Holladay, UT 84121, plus telehealth patients in 38 states. Phone (801) 893-6725 · support@getrenewrx.com. ~2,500+ patients treated; 5.0-star rating on 39 Google reviews; LegitScript verified; medications sourced from licensed 503A compounding pharmacies; labs rechecked every 90 days.

## Scope of Work

**Local Visibility — Google Business Profile and Lead Tracking**
- CRM Workspace
- Live reporting dashboard
- Google Business Profile optimization

**Paid Ads — Lead Generation**
- Paid Google search ads
- Paid Meta ads (Facebook + Instagram)
- Conversion landing page
- Call tracking for lead attribution

**Process:** 01 Discover → 02 Build → 03 Grow.

## Brand & Voice Notes

Clinical, direct, credibility-forward, slightly contrarian ("not a prescription mill, not an algorithm"), evidence-led (labs/licensure over hype). Recurring pillars: "Lab-guided care from licensed providers," "We recheck labs every 90 days," "Bridging the gap between patients and real clinical care."

### Brand block (authoritative — Brand Source Of Truth ladder, local-landing-page-builder v1.2.0)

Extracted 2026-08-14 via the governed `audit_brand_dna` request (Landing Page Builder extension, invoker INV_5e3cbc3d; `Palette Fallback: false`, `Font Fallback: false`). Supersedes the 2026-08-13 note that brand tokens could not be extracted.

```json
"brand": {
  "primary": "#c9a96e", "secondary": "#0b5d6e",
  "neutral_dark": "#1a1a1a", "neutral_light": "#ffffff",
  "highlight": "#0b5d6e",
  "heading_font": "IBM Plex Mono", "body_font": "Inter",
  "logo_url": null,
  "source": "extracted 2026-08-14 (audit_brand_dna)"
}
```

Not yet surfaced by the request (open extension item): logo URL, hero image URL, provider headshots — drafts use a styled text wordmark and brand-colored hero treatment until supplied.

## Delivery Log

| Date | Line | Deliverable | Commit | Krista Execution | Status |
|---|---|---|---|---|---|
| 2026-08-13 | Boost Engine | Provisioning (repo + Pages) | this commit | — | done |
| 2026-08-13 | Boost Engine | Signed MSA/SOW filed · docset: NVM_Contract_RenewRX_07292026.pdf | — | CEC_auto_e41110dd-5fbc-4266-b0ca-6d3347dc4208 | done |
| 2026-08-13 | Paid Ads | Conversion landing page draft (D6, GLP-1 Weight Loss, Holladay UT) — campaigns/2026-08-13-paid-ads-conversion-landing-page-draft.html | this commit | — | draft — NOT published (real-client-publishing hard gate unresolved; brand colors/fonts are fallback, pending real CSS pull) |
| 2026-08-14 | Paid Ads | Conversion landing page draft v2 (D6, REAL brand tokens via audit_brand_dna; hybrid skill+request build) — campaigns/2026-08-14-paid-ads-conversion-landing-page-draft.html · docset: renewrx-landing-page-draft-2026-08-14.txt | 0fed5e548a52a595d4d5357024b60c8aad6d49ce | — | draft — NOT published (real-client-publishing hard gate awaits approval; brand tokens REAL — supersedes 08-13 fallback draft) |

<!-- Delivery Log schema v2 (2026-07-10):
  Commit = git SHA of the delivering commit, or "—" when the deliverable produced no git artifact.
  Krista Execution = execution_id · task_id · report_id (whichever exist, "·"-separated; "—" for
  local skill runs with no Krista conversation). Every Krista conversation execution MUST log its
  IDs here in the same turn it completes, and the same record is written to the KME on the Krista
  side — commit SHA is the join key from Krista to git; task/report IDs are the join key from git
  to Krista. A run is not "done" until its identity exists in both stores. -->