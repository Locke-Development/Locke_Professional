# Locke Professional — API and Operation Trace, Part 1
**Private source:** `Amishgangsta/Locke-Professional`, deployed release commit `590032c66a12`. This is an inventory of declared operations, not a live invocation or guarantee of availability.

Paths are relative to their mounted routers; route wrappers, entitlements, environment configuration and required inputs can restrict access.

## `routes/auth.js` (16 operations)

| Method | Route path | Source line |
|---|---|---:|
| GET | `/ai-disclosure` | 94 |
| GET | `/auth/session` | 98 |
| GET | `/auth/mfa/status` | 102 |
| POST | `/auth/mfa/enroll` | 117 |
| POST | `/auth/mfa/verify` | 126 |
| POST | `/auth/preview-session` | 138 |
| POST | `/auth/register` | 156 |
| POST | `/auth/password` | 186 |
| POST | `/auth/login` | 195 |
| POST | `/auth/logout` | 206 |
| GET | `/auth/sessions` | 216 |
| POST | `/auth/sessions/:id/revoke` | 225 |
| POST | `/auth/password-reset` | 245 |
| POST | `/auth/password-reset/confirm` | 261 |
| POST | `/auth/email-verification` | 274 |
| POST | `/auth/verify-email` | 296 |

## `routes/contracts.js` (31 operations)

| Method | Route path | Source line |
|---|---|---:|
| GET | `/contracts/lifecycle` | 114 |
| GET | `/approvals/policy` | 130 |
| PUT | `/approvals/policy` | 138 |
| POST | `/contracts/:id/execute` | 153 |
| GET | `/contracts/:id/artifacts` | 185 |
| GET | `/artifacts/:artifactId/download` | 203 |
| GET | `/artifacts/verify` | 225 |
| GET | `/contracts/:id/lineage` | 233 |
| POST | `/contracts/:id/artifact-versions` | 241 |
| GET | `/lineage-artifacts/:artifactId/download` | 254 |
| POST | `/lineage-artifacts/:artifactId/legal-hold` | 270 |
| POST | `/contracts/:id/erasure` | 283 |
| POST | `/contracts/:id/restore` | 296 |
| GET | `/renewals` | 314 |
| GET | `/contracts/:id/terms` | 330 |
| PUT | `/contracts/:id/terms` | 340 |
| GET | `/contracts/:id/extraction-jobs` | 354 |
| POST | `/extraction-jobs/:jobId/retry` | 363 |
| POST | `/extraction-jobs/:jobId/cancel` | 372 |
| GET | `/contracts/:id/approvals` | 381 |
| POST | `/contracts/:id/approvals` | 392 |
| GET | `/contracts` | 415 |
| GET | `/contracts/facets` | 424 |
| POST | `/contracts` | 433 |
| GET | `/contracts/:id` | 453 |
| PATCH | `/contracts/:id/status` | 467 |
| GET | `/obligations` | 483 |
| PATCH | `/obligations/:id` | 492 |
| GET | `/contracts/:id/obligations` | 506 |
| POST | `/contracts/:id/draft-language` | 517 |
| POST | `/contracts/:id/extract-obligations` | 542 |

## `routes/documents.js` (3 operations)

| Method | Route path | Source line |
|---|---|---:|
| GET | `/documents/capabilities` | 17 |
| GET | `/documents/formats` | 26 |
| POST | `/documents/export` | 30 |

## `routes/intake.js` (9 operations)

| Method | Route path | Source line |
|---|---|---:|
| GET | `/statuses` | 102 |
| POST | `/` | 109 |
| GET | `/` | 132 |
| GET | `/assignees` | 146 |
| GET | `/:id` | 154 |
| POST | `/:id/supporting-document` | 166 |
| POST | `/:id/accept` | 181 |
| POST | `/:id/decline` | 191 |
| POST | `/:id/cancel` | 201 |

## `routes/external_intake.js` (5 operations)

| Method | Route path | Source line |
|---|---|---:|
| POST | `/intake-forms` | 38 |
| GET | `/intake-forms` | 45 |
| DELETE | `/intake-forms/:id` | 49 |
| GET | `/external-intake/form` | 53 |
| POST | `/external-intake/submit` | 57 |

## `routes/review.js` (34 operations)

| Method | Route path | Source line |
|---|---|---:|
| GET | `/review-rules` | 36 |
| POST | `/review-rules` | 41 |
| PATCH | `/review-rules/:ruleId` | 46 |
| DELETE | `/review-rules/:ruleId` | 54 |
| POST | `/reviews` | 61 |
| GET | `/reviews` | 73 |
| GET | `/reviews/:id` | 82 |
| DELETE | `/reviews/:id` | 92 |
| PATCH | `/reviews/:id` | 102 |
| GET | `/reviews/:id/findings` | 111 |
| POST | `/reviews/:id/findings` | 121 |
| PATCH | `/reviews/:id/findings/:findingId` | 130 |
| GET | `/reviews/:id/notes` | 139 |
| POST | `/reviews/:id/notes` | 149 |
| GET | `/reviews/:id/workspace` | 158 |
| GET | `/reviews/:id/items` | 168 |
| GET | `/reviews/:id/items/:findingId` | 178 |
| POST | `/reviews/:id/items/:findingId/decisions` | 188 |
| PATCH | `/reviews/:id/items/:findingId/assignment` | 198 |
| GET | `/reviews/:id/comments` | 208 |
| POST | `/reviews/:id/comments` | 218 |
| GET | `/reviews/:id/events` | 228 |
| POST | `/reviews/:id/items/:findingId/redlines` | 238 |
| GET | `/reviews/:id/exceptions` | 248 |
| POST | `/reviews/:id/items/:findingId/exceptions` | 256 |
| POST | `/reviews/:id/exceptions/:exceptionId/decision` | 264 |
| GET | `/reviews/:id/links` | 272 |
| POST | `/reviews/:id/items/:findingId/links` | 280 |
| POST | `/reviews/:id/compare` | 288 |
| GET | `/reviews/:id/completion-check` | 298 |
| POST | `/reviews/:id/complete` | 308 |
| GET | `/reviews/:id/document-versions` | 322 |
| POST | `/reviews/:id/document-versions` | 332 |
| POST | `/reviews/:id/items/:findingId/evidence` | 342 |

## `routes/guided_drafting.js` (12 operations)

| Method | Route path | Source line |
|---|---|---:|
| GET | `/guided-drafting/bootstrap` | 50 |
| GET | `/guided-drafting/templates/:templateId/questionnaire` | 58 |
| POST | `/guided-drafting/issue-spot` | 71 |
| GET | `/guided-drafting/registry/:libraryCode/validate` | 90 |
| POST | `/guided-drafting/matters` | 99 |
| POST | `/guided-drafting/matters/:matterId/decisions` | 119 |
| GET | `/guided-drafting/matters/:matterId/ledger` | 142 |
| POST | `/guided-drafting/custom-language` | 157 |
| POST | `/guided-drafting/party-relevance` | 182 |
| POST | `/guided-drafting/custom-agreement/analyze` | 191 |
| POST | `/guided-drafting/custom-agreement/recommend` | 202 |
| POST | `/guided-drafting/review/issue-spot` | 212 |

## `routes/library.js` (10 operations)

| Method | Route path | Source line |
|---|---|---:|
| GET | `/library` | 128 |
| GET | `/library/templates` | 137 |
| GET | `/library/clause-families` | 146 |
| GET | `/library/templates/:templateId` | 158 |
| GET | `/library/templates/:templateId/questionnaire` | 168 |
| POST | `/library/templates/:templateId/assemble` | 193 |
| POST | `/library/templates/:templateId/clearances` | 329 |
| GET | `/clause-types` | 408 |
| GET | `/playbooks` | 417 |
| GET | `/playbooks/:id/rules` | 426 |
