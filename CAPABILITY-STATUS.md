# Locke Professional — Tracked Capability Status

**Source:** `Amishgangsta/Locke-Professional` release commit `590032c66a12e6f67d47f925b48b581d30753ac4` (November 13, 2026).

The repository's own `data/feature-completeness.json` declares **24 capability families**. These are source-declared statuses, not new live end-to-end tests.

| # | Tracked capability | Declared status | Evidence paths | Qualification |
|---:|---|---|---|---|
| 1 | `authentication_account` | **complete** | `routes/auth.js`, `services/auth_session_service.js` | Tracked implementation; see detailed feature register. |
| 2 | `workspace_dashboard` | **complete** | `routes/dashboard.js`, `services/dashboard_service.js` | Tracked implementation; see detailed feature register. |
| 3 | `contract_repository` | **complete** | `routes/contracts.js`, `services/contracts_service.js` | Tracked implementation; see detailed feature register. |
| 4 | `document_import` | **complete** | `routes/documents.js`, `services/document_extract.js` | Tracked implementation; see detailed feature register. |
| 5 | `ocr` | **complete** | `routes/ocr.js`, `services/ocr_service.js` | Local OCR pipeline and corrections exist; environmental and quality gates apply. |
| 6 | `counterparty_review` | **complete** | `routes/guided_drafting.js`, `services/guided_drafting/issue_spotter.js` | Tracked implementation; see detailed feature register. |
| 7 | `document_compare` | **complete** | `routes/compare.js`, `services/text_compare.js` | Tracked implementation; see detailed feature register. |
| 8 | `guided_drafting` | **complete** | `routes/guided_drafting.js`, `services/guided_drafting/decision_ledger.js` | Tracked implementation; see detailed feature register. |
| 9 | `clause_library_assembly` | **complete** | `routes/library.js`, `services/agreement_library_service.js` | Tracked implementation; see detailed feature register. |
| 10 | `ai_drafting` | **complete** | `routes/drafting.js`, `services/contract_drafting.js` | Tracked implementation; see detailed feature register. |
| 11 | `ask_locke` | **complete** | `routes/chat.js`, `services/ask_locke_service.js` | Catalog routing, facts seeding, contract Q&A and excerpt-coverage note. |
| 12 | `jurisdiction_enrichment` | **complete** | `routes/jurisdiction.js`, `services/jurisdiction_gap_service.js` | Tracked implementation; see detailed feature register. |
| 13 | `obligations` | **complete** | `routes/contracts.js`, `services/obligation_extraction.js` | Tracked implementation; see detailed feature register. |
| 14 | `approval_gate` | **complete** | `routes/contracts.js`, `services/approval_service.js` | Tracked implementation; see detailed feature register. |
| 15 | `executed_artifacts` | **complete** | `routes/contracts.js`, `services/executed_artifact_service.js` | Tracked implementation; see detailed feature register. |
| 16 | `esign` | **complete** | `routes/esign.js`, `services/esign_service.js` | External recipient delivery depends on email configuration. |
| 17 | `document_export` | **complete** | `routes/documents.js`, `services/document_export_service.js` | Tracked implementation; see detailed feature register. |
| 18 | `renewals` | **incomplete** | `routes/contracts.js`, `services/renewal_service.js` | Notice-date calculations exist; public-holiday calendars and complete reminder delivery are not certified. |
| 19 | `intake` | **incomplete** | `routes/intake.js`, `services/intake_service.js` | Internal intake exists and external form routes exist, but the family remains incomplete. |
| 20 | `organizations` | **complete** | `routes/organizations.js`, `routes/admin.js` | Tracked implementation; see detailed feature register. |
| 21 | `email` | **incomplete** | `routes/auth.js`, `services/email_service.js` | Outbound delivery is provider-dependent and not certified across all message types. |
| 22 | `reports_usage_admin` | **incomplete** | `routes/admin.js`, `services/admin_service.js` | Admin and usage routes exist, but full reporting certification remains incomplete. |
| 23 | `domain_services` | **internal** | `routes/domain_services.js`, `services/cm_domain_client.js` | CM/PEA/TAF adapters exist; internal scope. |
| 24 | `billing` | **owner_decision_pending** | `routes/plans.js`, `routes/admin.js` | No demonstrated live checkout/subscription process; price list is planning-only. |

## Exact status counts
- **complete: 18**
- **incomplete: 4**
- **internal: 1**
- **owner_decision_pending: 1**

## Deployment and commercial distinction
Railway records a successful production deployment of the inspected SHA on November 12, 2026. That does not independently establish all external provider configurations, optional integrations or customer flows.

The public site describes **Professional, Professional Firm and Professional Enterprise**, with pricing by inquiry. The internal plan catalog explicitly warns its dollar values are planning anchors rather than published prices; subscription checkout remains unverified and is not presented as available.

## Library-count distinction
The live homepage source advertises **9 libraries and 99 templates ready for attorney review**. `libraries/registry.json` registers **13 packages**, but the live publication rule filters on `production_cleared`; registered does not mean customer-visible. These counts have not been reconciled against a newly executed production catalog query.

[Full atomic feature register](FEATURE-MATRIX.md) · [API route trace](ROUTE-TRACE.md) · [Methodology](METHODOLOGY.md)