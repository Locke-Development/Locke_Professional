# Locke Professional — API and Operation Trace, Part 2
**Source-verified declarations, not live functional tests.** Route path shown as declared; application mounts may prepend path segments.

## `routes/esign.js` (15 operations)

| Method | Route path | Source line |
|---|---|---:|
| GET | `/signing/external/session` | 85 |
| GET | `/signing/external/status` | 93 |
| POST | `/signing/external/otp/request` | 101 |
| POST | `/signing/external/otp/verify` | 121 |
| GET | `/signing/external/document` | 131 |
| POST | `/signing/external/sign` | 144 |
| POST | `/signing/external/decline` | 178 |
| GET | `/esign/capabilities` | 187 |
| GET | `/esign/requests` | 191 |
| POST | `/esign/requests` | 202 |
| GET | `/esign/requests/:id` | 227 |
| POST | `/esign/requests/:id/send` | 238 |
| POST | `/esign/requests/:id/sign` | 250 |
| GET | `/esign/requests/:id/certificate` | 275 |
| POST | `/esign/requests/:id/finalize` | 288 |

## `routes/ocr.js` (8 operations)

| Method | Route path | Source line |
|---|---|---:|
| GET | `/ocr/capabilities` | 35 |
| GET | `/ocr/jobs` | 39 |
| POST | `/ocr/upload` | 57 |
| POST | `/ocr/jobs` | 105 |
| GET | `/ocr/jobs/:id` | 126 |
| POST | `/ocr/jobs/:id/corrections` | 136 |
| POST | `/ocr/jobs/:id/understand` | 151 |
| POST | `/ocr/jobs/:id/accept` | 187 |

## `routes/drafting.js` (2 operations)

| Method | Route path | Source line |
|---|---|---:|
| GET | `/draft/status` | 42 |
| POST | `/draft` | 51 |

## `routes/chat.js` (1 operations)

| Method | Route path | Source line |
|---|---|---:|
| POST | `/chat` | 18 |

## `routes/compare.js` (1 operations)

| Method | Route path | Source line |
|---|---|---:|
| POST | `/compare` | 14 |

## `routes/admin.js` (13 operations)

| Method | Route path | Source line |
|---|---|---:|
| GET | `/overview` | 103 |
| GET | `/users` | 141 |
| GET | `/users/:id` | 157 |
| POST | `/users/:id/pro` | 176 |
| POST | `/users/:id/plan` | 187 |
| POST | `/users/:id/revoke-sessions` | 202 |
| GET | `/users/:id/organizations` | 225 |
| GET | `/organizations/:orgId/members` | 235 |
| POST | `/organizations/:orgId/members` | 245 |
| DELETE | `/organizations/:orgId/members/:userId` | 266 |
| GET | `/analytics` | 284 |
| GET | `/audit-log` | 293 |
| GET | `/billing/config` | 308 |

## `routes/organizations.js` (7 operations)

| Method | Route path | Source line |
|---|---|---:|
| GET | `/organizations` | 20 |
| GET | `/organizations/:orgId/approval-policy` | 35 |
| PUT | `/organizations/:orgId/approval-policy` | 43 |
| GET | `/organizations/:orgId/invites` | 51 |
| POST | `/organizations/:orgId/invites` | 59 |
| POST | `/organizations/:orgId/invites/:inviteId/revoke` | 73 |
| POST | `/organizations/invites/accept` | 85 |

## `routes/word_addin.js` (2 operations)

| Method | Route path | Source line |
|---|---|---:|
| GET | `/word/manifest.xml` | 132 |
| POST | `/word/session` | 138 |
