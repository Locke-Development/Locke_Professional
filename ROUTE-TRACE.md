# Locke Professional — Every Inspected API Route

This inventory traces source route declarations in 25 route modules, separately from the 361 customer-facing and technical capabilities in [FEATURE-MATRIX.md](FEATURE-MATRIX.md).

| Source section | Modules inspected | Declared operations | Link |
|---|---:|---:|---|
| Identity, contracts, imports, intake, review, guided drafting, library | 8 | 120 | [Part 1](ROUTE-TRACE-1.md) |
| E-sign, OCR, drafting, Ask Locke, comparison, administration, organizations, Word add-in | 8 | 49 | [Part 2](ROUTE-TRACE-2.md) |
| Webhooks, external collaboration, API keys, domain engines, dashboard, plans, product, jurisdiction, mounts | 9 | 34 | [Part 3](ROUTE-TRACE-3.md) |
| **TOTAL** | **25** | **203** | |

**Interpretation:** these are 203 static route-method declarations identified from source files, including routes implemented with multiple named routers; they do not represent 203 separate commercial features. Some are internal, preview, unconfigured, incomplete or subject to role checks. Router mount paths may prepend prefixes. The public portfolio does not test private credentials or execute operations.

See [CAPABILITY-STATUS.md](CAPABILITY-STATUS.md) for the exact tracked status of each family. Recent integrations, including the Word add-in and webhooks, are source-present but not deemed independently certified by this enumeration.

**Inspected release:** 590032c66a12e6f67d47f925b48b581d30753ac4. The privately held source code has not been copied into this public repository.
