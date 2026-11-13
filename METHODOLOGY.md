# Locke Professional — Research and Verification Method

**Audit date:** November 13, 2026.

## Locke evidence and deployment

- **Private source repository:** Amishgangsta/Locke-Professional.
- **Inspected branch:** release.
- **Inspected commit:** 590032c66a12e6f67d47f925b48b581d30753ac4.
- **Railway production:** service Locke-Professional, custom domains lockeprofessional.com and www.lockeprofessional.com, recorded SUCCESS deployment of the same commit on November 12, 2026.
- **Inventory basis:** data/feature-completeness.json (24 tracked capability families), services/capability_registry.js (runtime conditional capabilities), private routes and services (203 declarations across 25 inspected modules), professional-ui screens, and public product pages.
- **Ask Locke:** services/ask_locke_service.js, services/contract_chat.js, routes/chat.js, services/ai_output_schemas.js and public/lbc-chat-drawer.js.
- **Catalog:** libraries/registry.json plus services/catalog_release_policy.js; registered is different from production cleared.
- **Demo:** public/index.html references /guided-demo/locke-professional-demo.mp4 and /guided-demo/poster.jpg.

No new tests were requested or run; source and existing recorded CI/deployment information were reviewed.

## Current first-party competitor documentation

| Vendor | Official primary sources |
|---|---|
| Ironclad | [AI suite](https://ironcladapp.com/product/ironclad-ai), [Contract Review Agent](https://ironcladapp.com/product/review-contracts), [2026 product updates](https://academy.ironcladapp.com/pages/product-updates), [Playbooks](https://support.ironcladapp.com/hc/en-us/articles/12275685560215-Ironclad-AI-Playbooks-Overview) |
| Icertis | [Contract Management Platform](https://www.icertis.com/products/operate/contract-lifecycle-management/), [Vera Copilot](https://www.icertis.com/products/platform/copilot), [Obligations](https://www.icertis.com/products/operate/vera-obligations) |
| Agiloft | [Astra platform](https://www.agiloft.com/platform/astra), [November 5, 2026 agent update](https://www.agiloft.com/news/execution-focused-ai-agents) |
| LinkSquares | [Products](https://linksquares.com/products/linksquares-cloud/), [AI Legal Assistant](https://help.linksquares.com/hc/en-us/articles/41837640139927-AI-Legal-Assistant-for-Analyze-and-Finalize), [Word Add-In](https://help.linksquares.com/hc/en-us/articles/22984722372759-LinkSquares-Finalize-for-Word-Add-In-AI-Powered-Contract-Review) |
| Juro | [Products and AI](https://juro.com/lp), [2026 AI review updates](https://juro.com/product-updates/january-2026) |

## How comparisons are scored

- **●** = vendor publicly documents a comparable *feature category*, not verified one-to-one matching behavior.
- **≈** = relevant or adjacent vendor capability is documented; precise parity is unknown.
- **?** = no specific equivalent was verified; does not mean absent.
- **Locke ✓** = inspected source code directly supports an implementation.
- **Locke Partial / Conditional / Pending** = the source register or capability resolution explicitly limits availability.

A vendor is not declared inferior merely because a feature is not listed in the marketing documentation. Claims about performance, legal accuracy, legal sufficiency, total cost, uptime, security certifications and customer outcomes require evidence absent from this analysis.

## Independent facts and release caveats

**Exact 24-family source status:** 18 complete, 4 incomplete, 1 internal and 1 owner-decision-pending. The four source-incomplete areas are renewals, intake, outbound email, and reports/usage/admin certification; billing is awaiting commercial setup. Source-implemented means implemented **in code**, not that optional services are configured or a customer journey passed a new live test.

**Pricing:** Public tiers Professional, Professional Firm and Professional Enterprise are priced **by inquiry**. The private plan_catalog.js explicitly identifies internal pricing values as modeling anchors and describes a billing stub; they are not quoted as commercial prices.

**Template counts:** Public homepage text says 9 libraries/99 templates, while the private registry has 13 library packages. Release filtering is controlled by production_cleared; the portfolio distinguishes marketing claims, registered packages and live availability.

**Public/private boundaries:** proprietary source, clause text, internal security reports, customer contracts, API secrets, and configuration values were not copied to the public repository. Report filenames and general technical descriptions are provided for evidence traceability only.

[Brochure](BROCHURE.md) · [45-point comparison](COMPARISON.md) · [361-point feature register](FEATURE-MATRIX.md) · [203-route trace](ROUTE-TRACE.md)
