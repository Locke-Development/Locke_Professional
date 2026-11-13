# Locke Professional — API and Operation Trace, Part 3
**Source-verified route declarations, not a live transaction test.** Paths are relative to their application's router mounts.

## `routes/webhooks.js` (5 operations)

| Method | Route path | Source line |
|---|---|---:|
| GET | `/webhooks/events` | 19 |
| POST | `/webhooks` | 21 |
| GET | `/webhooks` | 25 |
| DELETE | `/webhooks/:id` | 29 |
| POST | `/webhooks/:id/test` | 33 |

## `routes/share_links.js` (6 operations)

| Method | Route path | Source line |
|---|---|---:|
| POST | `/contracts/:id/share-links` | 42 |
| GET | `/contracts/:id/share-links` | 49 |
| GET | `/contracts/:id/share-comments` | 53 |
| DELETE | `/share-links/:id` | 57 |
| GET | `/shared/contract` | 61 |
| POST | `/shared/comment` | 69 |

## `routes/api_keys.js` (3 operations)

| Method | Route path | Source line |
|---|---|---:|
| POST | `/api-keys` | 19 |
| GET | `/api-keys` | 23 |
| DELETE | `/api-keys/:id` | 27 |

## `routes/domain_services.js` (15 operations)

| Method | Route path | Source line |
|---|---|---:|
| GET | `/cm/domain/health` | 90 |
| POST | `/cm/domain/rights/evaluate-use` | 108 |
| POST | `/cm/domain/publication/check` | 124 |
| GET | `/cm/domain/assets/:assetVersionId/chain-of-title` | 140 |
| GET | `/pea/domain/health` | 160 |
| GET | `/pea/domain/jurisdictions` | 178 |
| POST | `/pea/domain/estates` | 191 |
| GET | `/pea/domain/estates/:estateId` | 205 |
| POST | `/pea/domain/estates/:estateId/documents/render` | 218 |
| GET | `/pea/domain/estates/:estateId/distribution-readiness` | 232 |
| GET | `/taf/domain/health` | 246 |
| GET | `/taf/domain/library/templates` | 264 |
| POST | `/taf/domain/trusts` | 277 |
| GET | `/taf/domain/trusts/:trustId` | 291 |
| POST | `/taf/domain/trusts/:trustId/documents/render` | 304 |

## `routes/dashboard.js` (1 operations)

| Method | Route path | Source line |
|---|---|---:|
| GET | `/dashboard/summary` | 9 |

## `routes/plans.js` (1 operations)

| Method | Route path | Source line |
|---|---|---:|
| GET | `/plans` | 9 |

## `routes/product.js` (1 operations)

| Method | Route path | Source line |
|---|---|---:|
| GET | `/product-disclaimer` | 13 |

## `routes/jurisdiction.js` (2 operations)

| Method | Route path | Source line |
|---|---|---:|
| GET | `/jurisdiction/status` | 14 |
| POST | `/jurisdiction/interpret` | 18 |

## `routes/business_contracts.js` (0 operations)

| Method | Route path | Source line |
|---|---|---:|
