# Locke Professional — Atomic Feature and Competitive Coverage Register
**Evidence snapshot:** private `Amishgangsta/Locke-Professional` branch `release` at `590032c66a12e6f67d47f925b48b581d30753ac4`; dated November 13, 2026. **Audience:** engineering employers and prospective software-development clients.

This register decomposes the product into **individual capabilities**, rather than counting a module name as proof of all its parts. It tracks every area declared in `data/feature-completeness.json` (24 areas), plus the separately inspected recent Integration surface. Each row is a source-identified capability, **not a separately executed customer test**. Some features have partial/incomplete family status; they are not represented as production-complete.

**Competitor columns:** I=Ironclad, C=Icertis, A=Agiloft, L=LinkSquares, J=Juro. `P` = a comparable *category* is published by that competitor, not exact feature equivalence; `R` = related published capability without confirmed parity; `?` = exact equivalent not verified. The source for the vendor columns is documented in [METHODOLOGY.md](METHODOLOGY.md). **No question mark denotes absence**. More specific comparisons appear in [COMPARISON.md](COMPARISON.md).

**Locke status:** `Complete*` means the source feature-completeness register describes that area as complete, *not* verified live end to end; `Partial*` means its area is explicitly incomplete; `Internal` means not a general user-facing promise; `Pending` means a commercial decision remains. Integration surface was inspected separately in current routes and is labeled `Source-implemented`.

## Identity, security and sessions (14 inspected items)
**Locke release status:** Complete*. **Code evidence:** `routes/auth.js`, `services/auth_session_service.js`, `services/auth_recovery_service.js`, `services/mfa_service.js`.

| # | Individual feature | Locke status | I | C | A | L | J |
|---:|---|---|:-:|:-:|:-:|:-:|:-:|
| 1 | Account registration | Complete* | R | R | R | R | R |
| 2 | Email/password sign-in | Complete* | R | R | R | R | R |
| 3 | HttpOnly workspace sessions | Complete* | R | R | R | R | R |
| 4 | Logout and session invalidation | Complete* | R | R | R | R | R |
| 5 | View active account sessions | Complete* | R | R | R | R | R |
| 6 | Revoke an individual session | Complete* | R | R | R | R | R |
| 7 | Change account password | Complete* | R | R | R | R | R |
| 8 | Password-reset request and token confirmation | Complete* | R | R | R | R | R |
| 9 | Email-verification token handling | Complete* | R | R | R | R | R |
| 10 | MFA enrollment | Complete* | R | R | R | R | R |
| 11 | MFA verification | Complete* | R | R | R | R | R |
| 12 | Login attempt throttling | Complete* | R | R | R | R | R |
| 13 | Same-origin mutation enforcement | Complete* | ? | ? | ? | ? | ? |
| 14 | Preview-account access separation | Complete* | ? | ? | ? | ? | ? |

## Dashboard and workspace navigation (9 inspected items)
**Locke release status:** Complete*. **Code evidence:** `routes/dashboard.js`, `services/dashboard_service.js`, `professional-ui/src/components/app/screens/Dashboard.tsx`, `professional-ui/src/components/app/App.tsx`.

| # | Individual feature | Locke status | I | C | A | L | J |
|---:|---|---|:-:|:-:|:-:|:-:|:-:|
| 15 | Authenticated workspace dashboard | Complete* | R | R | R | R | R |
| 16 | Organization-scoped contract count | Complete* | R | R | R | R | R |
| 17 | Open work and status summary | Complete* | R | R | R | R | R |
| 18 | Cross-module navigation | Complete* | R | R | R | R | R |
| 19 | Repository activity summary | Complete* | R | R | R | R | R |
| 20 | Contracts requiring review visibility | Complete* | R | R | R | R | R |
| 21 | Current obligation visibility | Complete* | R | R | R | R | R |
| 22 | Workspace access restrictions | Complete* | R | R | R | R | R |
| 23 | Live data refresh paths | Complete* | R | R | R | R | R |

## Contract repository and lifecycle (15 inspected items)
**Locke release status:** Complete*. **Code evidence:** `routes/contracts.js`, `services/contracts_service.js`, `services/contract_scope.js`, `services/contract_lifecycle.js`, `professional-ui/src/components/app/screens/ContractDetail.tsx`.

| # | Individual feature | Locke status | I | C | A | L | J |
|---:|---|---|:-:|:-:|:-:|:-:|:-:|
| 24 | Create contract record | Complete* | P | P | P | P | P |
| 25 | Contract title and counterparty data | Complete* | P | P | P | P | P |
| 26 | Record lifecycle status | Complete* | P | P | P | P | P |
| 27 | Record contract versions | Complete* | P | P | P | P | P |
| 28 | Search contracts within organization | Complete* | P | P | P | P | P |
| 29 | Filter contract facets | Complete* | P | P | P | P | P |
| 30 | Open contract details | Complete* | P | P | P | P | P |
| 31 | Update a contract | Complete* | P | P | P | P | P |
| 32 | Move contract between lifecycle states | Complete* | P | P | P | P | P |
| 33 | Reject invalid status transitions | Complete* | P | P | P | P | P |
| 34 | Preserve organization-level isolation | Complete* | P | P | P | P | P |
| 35 | Link documents to a contract | Complete* | P | P | P | P | P |
| 36 | Keep lifecycle event history | Complete* | P | P | P | P | P |
| 37 | Read-only API access to repository | Complete* | P | P | P | P | P |
| 38 | Contract list and detail user interface | Complete* | P | P | P | P | P |

## Document ingestion and preservation (10 inspected items)
**Locke release status:** Complete*. **Code evidence:** `routes/documents.js`, `services/document_extract.js`, `services/artifact_store.js`, `professional-ui/src/components/app/screens/Review.tsx`.

| # | Individual feature | Locke status | I | C | A | L | J |
|---:|---|---|:-:|:-:|:-:|:-:|:-:|
| 39 | PDF import | Complete* | P | P | P | P | P |
| 40 | DOCX import | Complete* | P | P | P | P | P |
| 41 | Plain-text document import | Complete* | P | P | P | P | P |
| 42 | Upload size enforcement | Complete* | P | P | P | P | P |
| 43 | MIME and file-content checks | Complete* | P | P | P | P | P |
| 44 | Extraction of embedded text | Complete* | P | P | P | P | P |
| 45 | Original source artifact retention | Complete* | ? | ? | ? | ? | ? |
| 46 | Organization-scoped artifact authorization | Complete* | ? | ? | ? | ? | ? |
| 47 | Text extraction failure reporting | Complete* | P | P | P | P | P |
| 48 | Contract-linked imported source | Complete* | P | P | P | P | P |

## Scans, OCR and evidence corrections (17 inspected items)
**Locke release status:** Complete*. **Code evidence:** `routes/ocr.js`, `services/ocr_service.js`, `services/ocr_worker.js`, `services/ocr_local_engine.js`, `services/ocr_quality.js`.

| # | Individual feature | Locke status | I | C | A | L | J |
|---:|---|---|:-:|:-:|:-:|:-:|:-:|
| 49 | Scanned PDF OCR | Complete* | R | P | R | P | R |
| 50 | Image OCR | Complete* | R | P | R | P | R |
| 51 | Local Tesseract processing | Complete* | R | P | R | P | R |
| 52 | Durable OCR job queue | Complete* | R | P | R | P | R |
| 53 | Check OCR job status | Complete* | R | P | R | P | R |
| 54 | List prior OCR jobs | Complete* | R | P | R | P | R |
| 55 | Lease-based worker claims | Complete* | ? | ? | ? | ? | ? |
| 56 | Bounded OCR retry and recovery | Complete* | ? | ? | ? | ? | ? |
| 57 | OCR text quality indicators | Complete* | ? | ? | ? | ? | ? |
| 58 | Review OCR extraction | Complete* | R | P | R | P | R |
| 59 | Correct OCR text | Complete* | ? | ? | ? | ? | ? |
| 60 | Accept corrected OCR output | Complete* | ? | ? | ? | ? | ? |
| 61 | Retain original scanned artifact | Complete* | R | P | R | P | R |
| 62 | Retain corrected and accepted artifact lineage | Complete* | ? | ? | ? | ? | ? |
| 63 | Document-understanding step | Complete* | R | P | R | P | R |
| 64 | Optional cloud provider adapter boundary | Complete* | ? | ? | ? | ? | ? |
| 65 | Malware-scan policy integration | Complete* | R | P | R | P | R |

## Attorney review and counterparty paper (25 inspected items)
**Locke release status:** Complete*. **Code evidence:** `routes/review.js`, `services/review_service.js`, `services/review_source_service.js`, `services/review_completion_service.js`, `professional-ui/src/components/app/screens/Review.tsx`.

| # | Individual feature | Locke status | I | C | A | L | J |
|---:|---|---|:-:|:-:|:-:|:-:|:-:|
| 66 | Create a review workspace | Complete* | P | P | P | P | P |
| 67 | Associate review with contract | Complete* | P | P | P | P | P |
| 68 | Choose represented party and posture | Complete* | P | P | P | P | P |
| 69 | Retain source document identity | Complete* | P | P | P | P | P |
| 70 | Version the reviewed document | Complete* | P | P | P | P | P |
| 71 | Detect and record issues | Complete* | P | P | P | P | P |
| 72 | Review severity and priority fields | Complete* | P | P | P | P | P |
| 73 | Add manual findings | Complete* | P | P | P | P | P |
| 74 | List review findings | Complete* | P | P | P | P | P |
| 75 | Assign reviewer | Complete* | ? | ? | ? | ? | ? |
| 76 | Set review due date | Complete* | P | P | P | P | P |
| 77 | Attach source text evidence | Complete* | P | P | P | P | P |
| 78 | Mark source verified or unverified | Complete* | ? | ? | ? | ? | ? |
| 79 | Decide individual findings | Complete* | P | P | P | P | P |
| 80 | Require reason for disposition | Complete* | ? | ? | ? | ? | ? |
| 81 | Add reviewer notes | Complete* | ? | ? | ? | ? | ? |
| 82 | Collaborative review comments | Complete* | P | P | P | P | P |
| 83 | Review event history | Complete* | P | P | P | P | P |
| 84 | Create proposed redline | Complete* | P | P | P | P | P |
| 85 | Submit exception request | Complete* | P | P | P | P | P |
| 86 | Decide exception request | Complete* | P | P | P | P | P |
| 87 | Link issues to related records | Complete* | P | P | P | P | P |
| 88 | Compare reviewed versions | Complete* | P | P | P | P | P |
| 89 | Completion blocker check | Complete* | P | P | P | P | P |
| 90 | Complete review with final disposition | Complete* | P | P | P | P | P |

## Compare and negotiation changes (8 inspected items)
**Locke release status:** Complete*. **Code evidence:** `routes/compare.js`, `services/text_compare.js`, `professional-ui/src/components/app/screens/Compare.tsx`, `public/lbc-compare.js`.

| # | Individual feature | Locke status | I | C | A | L | J |
|---:|---|---|:-:|:-:|:-:|:-:|:-:|
| 91 | Compare two contract versions | Complete* | P | P | P | P | P |
| 92 | Identify added text | Complete* | P | P | P | P | P |
| 93 | Identify removed text | Complete* | P | P | P | P | P |
| 94 | Bound the compared inputs | Complete* | ? | ? | ? | ? | ? |
| 95 | Render comparison safely | Complete* | P | P | P | P | P |
| 96 | Show changed text in reviewer UI | Complete* | ? | ? | ? | ? | ? |
| 97 | Keep compare within workspace access policy | Complete* | P | P | P | P | P |
| 98 | Create compare record from review | Complete* | P | P | P | P | P |

## Decision-led guided drafting (25 inspected items)
**Locke release status:** Complete*. **Code evidence:** `routes/guided_drafting.js`, `services/guided_drafting/issue_spotter.js`, `services/guided_drafting/decision_ledger.js`, `professional-ui/src/components/app/screens/CustomAgreement.tsx`.

| # | Individual feature | Locke status | I | C | A | L | J |
|---:|---|---|:-:|:-:|:-:|:-:|:-:|
| 99 | Start a governed drafting matter | Complete* | R | R | R | R | R |
| 100 | Describe a deal in ordinary language | Complete* | R | R | R | R | R |
| 101 | Classify agreement type | Complete* | R | R | R | R | R |
| 102 | Identify represented-party posture | Complete* | R | R | R | R | R |
| 103 | Collect canonical contract facts | Complete* | R | R | R | R | R |
| 104 | Select relevant template | Complete* | R | R | R | R | R |
| 105 | Load issue registry | Complete* | R | R | R | R | R |
| 106 | Ask decision-specific questions | Complete* | ? | ? | ? | ? | ? |
| 107 | Surface overlooked issues | Complete* | R | R | R | R | R |
| 108 | Show recommended clause position | Complete* | R | R | R | R | R |
| 109 | Show acceptable alternative positions | Complete* | R | R | R | R | R |
| 110 | Explain protected-party interest | Complete* | R | R | R | R | R |
| 111 | Expose risk of leaving issue unresolved | Complete* | R | R | R | R | R |
| 112 | Identify load-bearing decisions | Complete* | R | R | R | R | R |
| 113 | Accept recommended position | Complete* | R | R | R | R | R |
| 114 | Change or override a position | Complete* | R | R | R | R | R |
| 115 | Record custom language | Complete* | R | R | R | R | R |
| 116 | Persist attorney decision ledger | Complete* | R | R | R | R | R |
| 117 | Retrieve decision ledger after restart | Complete* | R | R | R | R | R |
| 118 | Associate decision with matter | Complete* | R | R | R | R | R |
| 119 | Record decision version/conflict | Complete* | R | R | R | R | R |
| 120 | Configure role-relevant terms | Complete* | R | R | R | R | R |
| 121 | Analyze custom agreement request | Complete* | R | R | R | R | R |
| 122 | Recommend custom agreement route | Complete* | R | R | R | R | R |
| 123 | Refuse unsupported assembly assumptions | Complete* | ? | ? | ? | ? | ? |

## Clause libraries, forms and assembly (20 inspected items)
**Locke release status:** Complete*. **Code evidence:** `routes/library.js`, `services/agreement_library_service.js`, `services/agreement_assembly_service.js`, `services/catalog_release_policy.js`.

| # | Individual feature | Locke status | I | C | A | L | J |
|---:|---|---|:-:|:-:|:-:|:-:|:-:|
| 124 | Browse governed library categories | Complete* | P | P | P | P | P |
| 125 | Browse templates by library | Complete* | P | P | P | P | P |
| 126 | Load individual template metadata | Complete* | P | P | P | P | P |
| 127 | Retrieve template questionnaire | Complete* | P | P | P | P | P |
| 128 | Identify clause families | Complete* | P | P | P | P | P |
| 129 | List clause types | Complete* | P | P | P | P | P |
| 130 | Open clause playbooks | Complete* | P | P | P | P | P |
| 131 | Inspect clause rule sets | Complete* | P | P | P | P | P |
| 132 | Associate clause with template | Complete* | P | P | P | P | P |
| 133 | Use production-cleared catalog filter | Complete* | ? | ? | ? | ? | ? |
| 134 | Withhold non-cleared template packages | Complete* | P | P | P | P | P |
| 135 | Load state-specific clause context | Complete* | ? | ? | ? | ? | ? |
| 136 | Assemble agreement from collected answers | Complete* | P | P | P | P | P |
| 137 | Run load-bearing review guard | Complete* | P | P | P | P | P |
| 138 | Surface warnings and approval conditions | Complete* | P | P | P | P | P |
| 139 | Render assembled agreement | Complete* | P | P | P | P | P |
| 140 | Apply structured clause variables | Complete* | P | P | P | P | P |
| 141 | Handle missing required inputs | Complete* | ? | ? | ? | ? | ? |
| 142 | Mark document output for attorney review | Complete* | P | P | P | P | P |
| 143 | Maintain independent domain library registration | Complete* | P | P | P | P | P |

## AI-supported drafting and jurisdiction (12 inspected items)
**Locke release status:** Complete*. **Code evidence:** `routes/drafting.js`, `services/contract_drafting.js`, `services/ai_model_config.js`, `services/ai_gateway.js`, `routes/jurisdiction.js`.

| # | Individual feature | Locke status | I | C | A | L | J |
|---:|---|---|:-:|:-:|:-:|:-:|:-:|
| 144 | Drafting assistance with approved model | Complete* | P | P | P | P | P |
| 145 | Structured AI response validation | Complete* | P | P | P | P | P |
| 146 | Model and provider provenance recording | Complete* | ? | ? | ? | ? | ? |
| 147 | Provider availability check | Complete* | ? | ? | ? | ? | ? |
| 148 | Bound prompt and response sizes | Complete* | ? | ? | ? | ? | ? |
| 149 | Per-request AI timeout | Complete* | P | P | P | P | P |
| 150 | Bounded transient-error retry | Complete* | ? | ? | ? | ? | ? |
| 151 | AI circuit breaker | Complete* | P | P | P | P | P |
| 152 | AI spending ceiling | Complete* | P | P | P | P | P |
| 153 | Jurisdiction enrichment request | Complete* | ? | ? | ? | ? | ? |
| 154 | Jurisdiction uncertainty disclosure | Complete* | ? | ? | ? | ? | ? |
| 155 | Distinguish attorney decision from AI recommendation | Complete* | P | P | P | P | P |

## Ask Locke — assistant and workflow routing (24 inspected items)
**Locke release status:** Complete*. **Code evidence:** `routes/chat.js`, `services/ask_locke_service.js`, `services/contract_chat.js`, `public/lbc-chat-drawer.js`, `services/ai_output_schemas.js`.

| # | Individual feature | Locke status | I | C | A | L | J |
|---:|---|---|:-:|:-:|:-:|:-:|:-:|
| 156 | Open contextual assistant drawer | Complete* | P | P | P | P | P |
| 157 | Understand current page and workflow stage | Complete* | P | P | P | P | P |
| 158 | Offer journey-stage next steps | Complete* | P | P | P | P | P |
| 159 | Interpret natural-language document need | Complete* | P | P | P | P | P |
| 160 | Locate actual library categories | Complete* | P | P | P | P | P |
| 161 | Suggest existing template | Complete* | P | P | P | P | P |
| 162 | Validate template ID | Complete* | P | P | P | P | P |
| 163 | Validate library code | Complete* | P | P | P | P | P |
| 164 | Ask for or process canonical deal facts | Complete* | P | P | P | P | P |
| 165 | Map facts into questionnaire seeds | Complete* | P | P | P | P | P |
| 166 | Carry facts into selected workflow | Complete* | P | P | P | P | P |
| 167 | Offer relevant navigation action | Complete* | P | P | P | P | P |
| 168 | Open template from suggestion | Complete* | P | P | P | P | P |
| 169 | Open review workflow from suggestion | Complete* | P | P | P | P | P |
| 170 | Differentiate product help from contract questions | Complete* | P | P | P | P | P |
| 171 | Answer questions against open contract text | Complete* | P | P | P | P | P |
| 172 | Disclose when only excerpt was read | Complete* | P | P | P | P | P |
| 173 | Avoid implying unsupported document coverage | Complete* | ? | ? | ? | ? | ? |
| 174 | Record assistant model/provider provenance | Complete* | ? | ? | ? | ? | ? |
| 175 | Use constrained JSON response structure | Complete* | P | P | P | P | P |
| 176 | Handle unavailable provider with deterministic fallback | Complete* | ? | ? | ? | ? | ? |
| 177 | Restrict template inventory for preview access | Complete* | P | P | P | P | P |
| 178 | Retain legal information/not-advice boundary | Complete* | ? | ? | ? | ? | ? |
| 179 | Control assistant input length | Complete* | P | P | P | P | P |

## Obligations and post-execution extraction (15 inspected items)
**Locke release status:** Complete*. **Code evidence:** `routes/contracts.js`, `services/obligation_extraction.js`, `services/extraction_worker.js`, `services/obligation_complexity.js`.

| # | Individual feature | Locke status | I | C | A | L | J |
|---:|---|---|:-:|:-:|:-:|:-:|:-:|
| 180 | Extract obligations after contract execution | Complete* | P | P | P | P | P |
| 181 | Queue extraction outside execution transaction | Complete* | P | P | P | P | P |
| 182 | Track extraction job status | Complete* | P | P | P | P | P |
| 183 | Retry failed extraction jobs | Complete* | P | P | P | P | P |
| 184 | Cancel queued extraction job | Complete* | P | P | P | P | P |
| 185 | Extract obligation source passage | Complete* | ? | ? | ? | ? | ? |
| 186 | Normalize obligation record | Complete* | ? | ? | ? | ? | ? |
| 187 | Record responsible party | Complete* | P | P | P | P | P |
| 188 | Record due date | Complete* | P | P | P | P | P |
| 189 | Track obligation status | Complete* | P | P | P | P | P |
| 190 | Filter obligations across contracts | Complete* | P | P | P | P | P |
| 191 | View obligations for one agreement | Complete* | P | P | P | P | P |
| 192 | Update obligation details | Complete* | P | P | P | P | P |
| 193 | Preserve AI provenance on extraction | Complete* | P | P | P | P | P |
| 194 | Bound extraction chunk workload | Complete* | ? | ? | ? | ? | ? |

## Approvals, separation of duties and gating (13 inspected items)
**Locke release status:** Complete*. **Code evidence:** `services/approval_service.js`, `services/contract_lifecycle.js`, `routes/contracts.js`, `routes/organizations.js`.

| # | Individual feature | Locke status | I | C | A | L | J |
|---:|---|---|:-:|:-:|:-:|:-:|:-:|
| 195 | Set approval required policy | Complete* | ? | ? | ? | ? | ? |
| 196 | Set organization approval policy | Complete* | P | P | P | P | P |
| 197 | Request internal approval | Complete* | P | P | P | P | P |
| 198 | Approve draft contract | Complete* | P | P | P | P | P |
| 199 | Reject submitted approval | Complete* | P | P | P | P | P |
| 200 | Record approver and comment | Complete* | P | P | P | P | P |
| 201 | Bind approval to source-text hash | Complete* | ? | ? | ? | ? | ? |
| 202 | Invalidate approval after text change | Complete* | P | P | P | P | P |
| 203 | Block signature when approval absent | Complete* | P | P | P | P | P |
| 204 | Require another approver for multi-person firm | Complete* | ? | ? | ? | ? | ? |
| 205 | Allow solo counsel path where applicable | Complete* | P | P | P | P | P |
| 206 | Expose current approval state to UI | Complete* | P | P | P | P | P |
| 207 | Enforce approval checks on e-sign creation | Complete* | P | P | P | P | P |

## Executed agreement records and lineage (11 inspected items)
**Locke release status:** Complete*. **Code evidence:** `services/executed_artifact_service.js`, `services/artifact_lineage_service.js`, `routes/contracts.js`.

| # | Individual feature | Locke status | I | C | A | L | J |
|---:|---|---|:-:|:-:|:-:|:-:|:-:|
| 208 | Upload externally executed copy | Complete* | P | P | P | P | P |
| 209 | Keep signed document in contract record | Complete* | P | P | P | P | P |
| 210 | Generate or persist content hash | Complete* | ? | ? | ? | ? | ? |
| 211 | Verify signed artifact hash on download | Complete* | ? | ? | ? | ? | ? |
| 212 | List executed artifacts | Complete* | P | P | P | P | P |
| 213 | Download authorized executed artifact | Complete* | P | P | P | P | P |
| 214 | Preserve original and derived artifact lineage | Complete* | ? | ? | ? | ? | ? |
| 215 | Enable legal hold control | Complete* | P | P | P | P | P |
| 216 | Soft-delete contract with controls | Complete* | P | P | P | P | P |
| 217 | Restore deleted contract | Complete* | P | P | P | P | P |
| 218 | Process configured erasure workflow | Complete* | P | P | P | P | P |

## Electronic signing and external recipients (17 inspected items)
**Locke release status:** Complete*. **Code evidence:** `routes/esign.js`, `services/esign_service.js`, `services/esign_recipient_service.js`, `services/esign_certificate_service.js`.

| # | Individual feature | Locke status | I | C | A | L | J |
|---:|---|---|:-:|:-:|:-:|:-:|:-:|
| 219 | Create signing request | Complete* | P | P | P | P | P |
| 220 | Attach authorized contract content | Complete* | P | P | P | P | P |
| 221 | Check required approval before signing | Complete* | ? | ? | ? | ? | ? |
| 222 | List signing requests | Complete* | P | P | P | P | P |
| 223 | View signing request state | Complete* | P | P | P | P | P |
| 224 | Send signing request | Complete* | P | P | P | P | P |
| 225 | Signer selection and recipient scope | Complete* | P | P | P | P | P |
| 226 | Typed or drawn signature collection | Complete* | P | P | P | P | P |
| 227 | External recipient signing link | Complete* | P | P | P | P | P |
| 228 | External recipient OTP request | Complete* | P | P | P | P | P |
| 229 | External recipient OTP verification | Complete* | P | P | P | P | P |
| 230 | Externally hosted document view | Complete* | P | P | P | P | P |
| 231 | Recipient accepts or declines | Complete* | P | P | P | P | P |
| 232 | Finalize signing request | Complete* | P | P | P | P | P |
| 233 | Create signing certificate | Complete* | P | P | P | P | P |
| 234 | Preserve signing event and hash binding | Complete* | ? | ? | ? | ? | ? |
| 235 | Signing degraded state when email unavailable | Complete* | ? | ? | ? | ? | ? |

## Document format support and downloads (11 inspected items)
**Locke release status:** Complete*. **Code evidence:** `routes/documents.js`, `services/document_export_service.js`, `services/pdf_render.js`, `services/artifact_store.js`.

| # | Individual feature | Locke status | I | C | A | L | J |
|---:|---|---|:-:|:-:|:-:|:-:|:-:|
| 236 | Export PDF | Complete* | P | P | P | P | P |
| 237 | Export DOCX | Complete* | P | P | P | P | P |
| 238 | Export RTF | Complete* | P | P | P | P | P |
| 239 | Export ODT | Complete* | P | P | P | P | P |
| 240 | Export HTML | Complete* | P | P | P | P | P |
| 241 | Export Markdown | Complete* | P | P | P | P | P |
| 242 | Export plain text | Complete* | P | P | P | P | P |
| 243 | Preserve complete source text during export | Complete* | P | P | P | P | P |
| 244 | Reject oversized export | Complete* | P | P | P | P | P |
| 245 | Enforce authorized download scope | Complete* | P | P | P | P | P |
| 246 | Attach export to agreement lifecycle | Complete* | P | P | P | P | P |

## Terms, renewals, notices and reminders (16 inspected items)
**Locke release status:** Partial*. **Code evidence:** `services/renewal_service.js`, `services/renewal_dates.js`, `services/renewal_reminder_service.js`, `routes/contracts.js`.

| # | Individual feature | Locke status | I | C | A | L | J |
|---:|---|---|:-:|:-:|:-:|:-:|:-:|
| 247 | Record term start date | Partial* | P | P | P | P | P |
| 248 | Record term end date | Partial* | P | P | P | P | P |
| 249 | Record renewal type | Partial* | P | P | P | P | P |
| 250 | Record notice period | Partial* | P | P | P | P | P |
| 251 | Record calendar/business day basis | Partial* | P | P | P | P | P |
| 252 | Compute nonrenewal notice date | Partial* | P | P | P | P | P |
| 253 | Show upcoming renewal candidates | Partial* | P | P | P | P | P |
| 254 | Bound renewal-search scan | Partial* | ? | ? | ? | ? | ? |
| 255 | Prevent invalid contract dates | Partial* | P | P | P | P | P |
| 256 | Report uncertain or incomplete term facts | Partial* | P | P | P | P | P |
| 257 | Compute weekends in business-day calculation | Partial* | P | P | P | P | P |
| 258 | Apply jurisdiction-specific holiday calendar | Partial* | ? | ? | ? | ? | ? |
| 259 | Schedule renewal notice stages | Partial* | P | P | P | P | P |
| 260 | Queue deduplicated renewal notification | Partial* | P | P | P | P | P |
| 261 | Deliver reminder with provider confirmation | Partial* | ? | ? | ? | ? | ? |
| 262 | Record delivery acknowledgement | Partial* | P | P | P | P | P |

## Internal and external contract requests (16 inspected items)
**Locke release status:** Partial*. **Code evidence:** `routes/intake.js`, `routes/external_intake.js`, `services/intake_service.js`, `services/external_intake_service.js`.

| # | Individual feature | Locke status | I | C | A | L | J |
|---:|---|---|:-:|:-:|:-:|:-:|:-:|
| 263 | Submit internal contract request | Partial* | P | P | P | P | P |
| 264 | Classify intake priority | Partial* | P | P | P | P | P |
| 265 | Record counterparty details | Partial* | P | P | P | P | P |
| 266 | Assign intake request | Partial* | P | P | P | P | P |
| 267 | List and filter intake queue | Partial* | P | P | P | P | P |
| 268 | Retrieve one intake request | Partial* | P | P | P | P | P |
| 269 | Attach supporting document | Partial* | P | P | P | P | P |
| 270 | Accept request and create draft | Partial* | P | P | P | P | P |
| 271 | Decline request with reason | Partial* | P | P | P | P | P |
| 272 | Cancel/withdraw request | Partial* | P | P | P | P | P |
| 273 | Create external intake form | Partial* | P | P | P | P | P |
| 274 | Issue external access token | Partial* | P | P | P | P | P |
| 275 | Revoke external intake form | Partial* | P | P | P | P | P |
| 276 | Submit intake through token | Partial* | P | P | P | P | P |
| 277 | Quarantine external supporting files | Partial* | P | P | P | P | P |
| 278 | Demonstrate configured end-to-end external intake | Partial* | ? | ? | ? | ? | ? |

## Firms, teams and collaboration governance (13 inspected items)
**Locke release status:** Complete*. **Code evidence:** `routes/organizations.js`, `services/contract_scope.js`, `services/organization_invite_service.js`, `routes/admin.js`.

| # | Individual feature | Locke status | I | C | A | L | J |
|---:|---|---|:-:|:-:|:-:|:-:|:-:|
| 279 | Create and manage organization context | Complete* | P | P | P | P | P |
| 280 | Organization-scoped repository data | Complete* | P | P | P | P | P |
| 281 | List organization memberships | Complete* | P | P | P | P | P |
| 282 | Invite member by email when configured | Complete* | P | P | P | P | P |
| 283 | Accept organization invitation | Complete* | P | P | P | P | P |
| 284 | Revoke pending invitation | Complete* | P | P | P | P | P |
| 285 | Assign owner/counsel/approver roles | Complete* | P | P | P | P | P |
| 286 | Remove organization member | Complete* | P | P | P | P | P |
| 287 | Share clauses and agreement records within firm | Complete* | P | P | P | P | P |
| 288 | Configure organization approval policy | Complete* | P | P | P | P | P |
| 289 | Enforce separation of duties | Complete* | ? | ? | ? | ? | ? |
| 290 | Check cross-tenant object access | Complete* | P | P | P | P | P |
| 291 | Manage firm-member permissions | Complete* | P | P | P | P | P |

## Outbound email and notifications (9 inspected items)
**Locke release status:** Partial*. **Code evidence:** `services/email_service.js`, `services/outbound_message_service.js`, `routes/auth.js`, `services/renewal_reminder_service.js`.

| # | Individual feature | Locke status | I | C | A | L | J |
|---:|---|---|:-:|:-:|:-:|:-:|:-:|
| 292 | Send account verification email | Partial* | P | P | P | P | P |
| 293 | Send password reset email | Partial* | P | P | P | P | P |
| 294 | Send organization invitation | Partial* | P | P | P | P | P |
| 295 | Send signing invitation | Partial* | P | P | P | P | P |
| 296 | Send outside signer OTP | Partial* | P | P | P | P | P |
| 297 | Queue outbound messages | Partial* | ? | ? | ? | ? | ? |
| 298 | Retry provider delivery | Partial* | ? | ? | ? | ? | ? |
| 299 | Send renewal notifications | Partial* | P | P | P | P | P |
| 300 | Manage unavailable outbound provider state | Partial* | ? | ? | ? | ? | ? |

## Reporting, usage, support and governance (13 inspected items)
**Locke release status:** Partial*. **Code evidence:** `routes/admin.js`, `services/admin_service.js`, `services/usage_service.js`, `professional-ui/src/components/app/screens/Admin.tsx`.

| # | Individual feature | Locke status | I | C | A | L | J |
|---:|---|---|:-:|:-:|:-:|:-:|:-:|
| 301 | Administrator overview | Partial* | P | P | P | P | P |
| 302 | Search users | Partial* | P | P | P | P | P |
| 303 | Inspect individual account | Partial* | P | P | P | P | P |
| 304 | Assign or revoke Pro access manually | Partial* | P | P | P | P | P |
| 305 | Change plan code administratively | Partial* | P | P | P | P | P |
| 306 | Force session revocation | Partial* | P | P | P | P | P |
| 307 | Manage firm members | Partial* | P | P | P | P | P |
| 308 | View administrative audit log | Partial* | ? | ? | ? | ? | ? |
| 309 | View AI usage and provider cost metrics | Partial* | ? | ? | ? | ? | ? |
| 310 | View aggregated workspace analytics | Partial* | P | P | P | P | P |
| 311 | View reporting dashboard | Partial* | P | P | P | P | P |
| 312 | Expose billing configuration status to admin | Partial* | P | P | P | P | P |
| 313 | Verify complete admin/report certification | Partial* | ? | ? | ? | ? | ? |

## Specialized domain packages and independent engines (14 inspected items)
**Locke release status:** Internal. **Code evidence:** `routes/domain_services.js`, `services/cm_domain_client.js`, `services/pea_domain_client.js`, `services/taf_domain_client.js`, `contracts/domain-services/v1.json`.

| # | Individual feature | Locke status | I | C | A | L | J |
|---:|---|---|:-:|:-:|:-:|:-:|:-:|
| 314 | Creative and marketing IP clause package | Internal | ? | ? | ? | ? | ? |
| 315 | Creative assets rights evaluation | Internal | ? | ? | ? | ? | ? |
| 316 | Publication checks and approval chain | Internal | ? | ? | ? | ? | ? |
| 317 | Chain-of-title lookup | Internal | ? | ? | ? | ? | ? |
| 318 | Rights and royalty rules in domain engine | Internal | ? | ? | ? | ? | ? |
| 319 | Private estate administration jurisdiction list | Internal | ? | ? | ? | ? | ? |
| 320 | Estate record creation | Internal | ? | ? | ? | ? | ? |
| 321 | Estate document rendering | Internal | ? | ? | ? | ? | ? |
| 322 | Estate distribution-readiness check | Internal | ? | ? | ? | ? | ? |
| 323 | Trusts and fiduciary template list | Internal | ? | ? | ? | ? | ? |
| 324 | Trust record creation | Internal | ? | ? | ? | ? | ? |
| 325 | Trust document rendering | Internal | ? | ? | ? | ? | ? |
| 326 | Independent domain-service health | Internal | ? | ? | ? | ? | ? |
| 327 | HMAC service-to-service identity controls | Internal | ? | ? | ? | ? | ? |

## Commercial subscription operations (10 inspected items)
**Locke release status:** Pending. **Code evidence:** `routes/plans.js`, `services/plan_catalog.js`, `routes/admin.js`, `public/pricing.html`.

| # | Individual feature | Locke status | I | C | A | L | J |
|---:|---|---|:-:|:-:|:-:|:-:|:-:|
| 328 | Publish consultation-led pricing tiers | Pending | P | P | P | P | P |
| 329 | Advertise Professional individual plan | Pending | P | P | P | P | P |
| 330 | Advertise Professional Firm plan | Pending | P | P | P | P | P |
| 331 | Advertise Professional Enterprise plan | Pending | P | P | P | P | P |
| 332 | Store plan feature flags | Pending | P | P | P | P | P |
| 333 | Assign access through admin | Pending | P | P | P | P | P |
| 334 | Create live Stripe checkout | Pending | ? | ? | ? | ? | ? |
| 335 | Reconcile Stripe webhooks | Pending | ? | ? | ? | ? | ? |
| 336 | Automatically provision paid seat | Pending | ? | ? | ? | ? | ? |
| 337 | Verify plan billing invoices | Pending | ? | ? | ? | ? | ? |

## Integration surfaces and extensibility (24 inspected items)
**Locke release status:** Source-implemented. **Code evidence:** `routes/api_keys.js`, `services/api_key_service.js`, `routes/webhooks.js`, `services/webhook_service.js`, `routes/share_links.js`, `routes/word_addin.js`.

| # | Individual feature | Locke status | I | C | A | L | J |
|---:|---|---|:-:|:-:|:-:|:-:|:-:|
| 338 | Issue scoped read-only API key | Source-implemented | P | P | P | P | P |
| 339 | List issued API keys | Source-implemented | P | P | P | P | P |
| 340 | Revoke API key | Source-implemented | P | P | P | P | P |
| 341 | Restrict token to GET/HEAD | Source-implemented | P | P | P | P | P |
| 342 | Allowlist API-key readable resources | Source-implemented | P | P | P | P | P |
| 343 | Create outbound webhook destination | Source-implemented | ? | ? | ? | ? | ? |
| 344 | List webhook subscriptions | Source-implemented | P | P | P | P | P |
| 345 | Revoke webhook | Source-implemented | P | P | P | P | P |
| 346 | Emit contract-created event | Source-implemented | P | P | P | P | P |
| 347 | Emit intake-submitted event | Source-implemented | P | P | P | P | P |
| 348 | Emit signature-completed event | Source-implemented | P | P | P | P | P |
| 349 | Emit renewal-notice-due event | Source-implemented | P | P | P | P | P |
| 350 | HMAC-sign webhook payload | Source-implemented | P | P | P | P | P |
| 351 | Queue and retry webhook delivery | Source-implemented | P | P | P | P | P |
| 352 | Reject private-address/SSRF targets | Source-implemented | P | P | P | P | P |
| 353 | Send test webhook | Source-implemented | P | P | P | P | P |
| 354 | Generate Microsoft Word add-in manifest | Source-implemented | P | P | P | P | P |
| 355 | Exchange authenticated session for add-in token | Source-implemented | P | P | P | P | P |
| 356 | Open Word task pane | Source-implemented | P | P | P | P | P |
| 357 | Review document from Word | Source-implemented | P | P | P | P | P |
| 358 | Insert governed clause in Word | Source-implemented | P | P | P | P | P |
| 359 | Save changes into Locke record | Source-implemented | P | P | P | P | P |
| 360 | Create revocable external review share-link | Source-implemented | P | P | P | P | P |
| 361 | Accept external review comments | Source-implemented | P | P | P | P | P |

## Completeness summary

- **361 atomic feature lines** inventoried in 24 source-mapped families. The 24 family statuses match the application's tracked feature register; Integration is a separately observed expansion.
- **18 tracked complete; 4 incomplete; 1 internal; 1 owner-decision pending.** Complete means source-declared, not a tested production guarantee.
- No source internals, private customer records, API keys or clause-bank text are reproduced.
- See [ROUTE-TRACE.md](ROUTE-TRACE.md) for the endpoint-by-endpoint register, including route operations not treated as marketing features.
