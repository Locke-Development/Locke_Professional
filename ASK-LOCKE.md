# ASK LOCKE — A COMPLETE ENGINEERING AND COMPETITIVE REVIEW
## Contextual intelligence that advances a contract workflow without pretending to be the attorney

**Reviewed:** November 13, 2026 · **Source:** Locke Professional private repository, release commit 590032c66a12 · **Audience:** software development clients and engineering employers.

Ask Locke is not just a chat widget. Its current implementation **separates product navigation and real-template recommendations from contract-grounded question answering**, adjusts to the current workflow stage, and can carry canonical deal facts into governed questionnaires. Its most important control is honesty about incomplete document context.

## How it works

### 1. Navigate an actual product
Ask Locke interprets the person's request and page context, infers their place in the journey, and offers valid destinations: library, template, draft, review, dates, risks, obligations and reports. Recommendations are parsed against currently registered library codes and template IDs; preview users receive category-level guidance without the full production template listing.

### 2. Turn useful facts into controlled fields
The assistant's fact schema includes parties, state/county/city, dates, monetary values, contract type and represented-party posture. It maps supported canonical facts to known questionnaire variable names—actual product handoff rather than free-form advice in a disconnected chat.

### 3. Answer against the agreement being reviewed
When substantive questions are asked with an open contract, Ask Locke uses bounded contract content through its dedicated question-answering service. If the model received only part of the agreement, the answer itself warns that it **cannot confirm an issue is absent from unread portions**. Product help remains on its navigation path.

### 4. Restrict the AI's authority
Recommendations are schema-validated and cannot invent a registered library or template. Message history is bounded, provider/model metadata is tracked, provider outages receive controlled fallback responses, and the product explicitly reserves final drafting/legal judgment for counsel.

## All 30 individually inspected Ask Locke behaviors

Legend: **●** published broadly comparable competitor AI capability; **≈** related capability, exact parity not checked; **?** no verified exact competitor detail. No question mark claims a feature is absent.

| # | Individual Ask Locke behavior | Locke | Ironclad | Icertis | Agiloft | LinkSquares | Juro | Finding |
|---:|---|:-:|:-:|:-:|:-:|:-:|:-:|---|
| 1 | Contextual sidebar access | ✓ | ● | ● | ● | ● | ● | All five publish in-workflow AI access |
| 2 | Current page awareness | ✓ | ≈ | ≈ | ≈ | ≈ | ≈ | Locke stage explicitly supplied; exact context paths vary |
| 3 | Journey stage inference | ✓ | ≈ | ≈ | ≈ | ≈ | ≈ | Specific Locke implementation confirmed |
| 4 | Stage-specific next-step guidance | ✓ | ● | ● | ● | ● | ● | AI guidance and task suggestions are common |
| 5 | Natural-language situation intake | ✓ | ● | ● | ● | ● | ● | Tie on intent understanding |
| 6 | Real library category recommendation | ✓ | ≈ | ≈ | ≈ | ≈ | ≈ | Recommendation checked against real library codes |
| 7 | Real template identifier recommendation | ✓ | ≈ | ≈ | ≈ | ≈ | ≈ | Template ID validated, not free-form |
| 8 | Preview-account catalog limitation | ✓ | ? | ? | ? | ? | ? | No competitor-specific preview restriction confirmed |
| 9 | Recognize contract-review question | ✓ | ● | ● | ● | ● | ● | Matter/document-based Q&A is mainstream |
| 10 | Distinguish navigation from substantive Q&A | ✓ | ≈ | ≈ | ≈ | ≈ | ≈ | Locke route selection verified |
| 11 | Read current contract source excerpt | ✓ | ● | ● | ● | ● | ● | Tie on source-grounded answers |
| 12 | Include clause reference in answer | ✓ | ● | ● | ● | ● | ● | Several peers cite clauses and sources |
| 13 | Disclose partial document reading | ✓ | ? | ? | ? | ? | ? | Source shows explicit coverage warning; no comparative proof |
| 14 | Avoid claiming absence in unread text | ✓ | ? | ? | ? | ? | ? | Explicit safeguard on excerpt-limited search |
| 15 | Canonical party A/B fact extraction | ✓ | ≈ | ≈ | ≈ | ≈ | ≈ | Locke fact mapping confirmed |
| 16 | State/county/city fact handling | ✓ | ≈ | ≈ | ≈ | ≈ | ≈ | Locke canonical fields confirmed |
| 17 | Date and amount seeding | ✓ | ≈ | ≈ | ≈ | ≈ | ≈ | Seed map confirmed |
| 18 | Represented party/role context | ✓ | ≈ | ≈ | ≈ | ≈ | ≈ | Posture integration verified |
| 19 | Map canonical facts to form variables | ✓ | ≈ | ≈ | ≈ | ≈ | ≈ | Actual engine inputs, not just chat memory |
| 20 | Structured recommendation response | ✓ | ≈ | ≈ | ≈ | ≈ | ≈ | Constrained parser and output schema |
| 21 | Navigation actions to relevant modules | ✓ | ● | ● | ● | ● | ● | Competitors publish task/workflow invocations |
| 22 | Fallback when provider unavailable | ✓ | ? | ? | ? | ? | ? | Deterministic fallback, no peer reliability comparison |
| 23 | Bound chat turn count and message length | ✓ | ? | ? | ? | ? | ? | Source has limits; peer internals not audited |
| 24 | Model/provider response provenance | ✓ | ≈ | ≈ | ≈ | ≈ | ≈ | Provider metadata recorded by Locke |
| 25 | Restrict to registered libraries/templates | ✓ | ≈ | ≈ | ≈ | ≈ | ≈ | Specific safety boundary |
| 26 | Keep attorney decision authority | ✓ | ● | ● | ● | ● | ● | Human oversight is present across the category |
| 27 | Separate AI drafting from governed assembly | ✓ | ≈ | ≈ | ≈ | ≈ | ≈ | Locke specific architectural separation |
| 28 | Do not represent assistant as legal counsel | ✓ | ● | ● | ● | ● | ● | Boundary is common |
| 29 | Route to review, risks, dates, obligations | ✓ | ● | ● | ● | ● | ● | Workflow context/action features exist elsewhere |
| 30 | Respond with product guidance when no contract loaded | ✓ | ≈ | ≈ | ≈ | ≈ | ≈ | Confirmed fallback path |

## Comparison against each rival assistant

- **Ironclad Agent and Contract Review Agent:** strong conversational access to contracts, AI-guided intake and playbooks, context-aware redlining and AI workflow invocation. Locke does **not** lead simply by being conversational; its value is the visible recommendation/facts/decision handoff.
- **Icertis Vera Copilot:** searches contracts and obligations, initiates workflows, uses playbooks and logs AI actions. Locke's stage-aware route and template validation are inspectable implementation choices, not a demonstrated capability gap at Icertis.
- **Agiloft Ask AI / Astra:** supports conversational contract interaction, record updates and specialized agents for contract requests and signatures. Locke offers a particular governed drafting front end; no blanket superiority claim is established.
- **LinkSquares AI Legal Assistant:** can ground reviews in up to five agreements, draft amendments, apply tracked redlines and research with citation-backed sources. Locke's source-excerpt warning is notable; LinkSquares has documented advanced review functionality Locke should not obscure.
- **Juro AI Assistant:** document drafting, summarizing, reviewing and extracting inside an integrated browser-native contract workflow. Ask Locke's strong point is its decision-led guidance and platform-specific routing, not novel use of an LLM.

## Four realistic demonstrations for an engineering interview

**A — Start with an unfamiliar deal.** Ask Locke for a contract type based on a free-text description; inspect which *real* library/template it recommends and what facts are carried forward.

**B — Review an imported agreement.** Ask about a termination or indemnification clause. The response should reflect the available contract text and explicitly indicate if coverage was truncated.

**C — Switch purpose mid-chat.** Ask to open the review workflow rather than seek legal analysis. The assistant should use product navigation, not pretend the contract itself answers the navigation question.

**D — Disconnect the AI provider.** The service contains a deterministic fallback so product discovery/navigation can remain useful without fabricated legal answers. This demonstrates failure-aware engineering; this publication did not execute a new outage test.

## Source inspection

Implementation paths examined: services/ask_locke_service.js; services/contract_chat.js; services/ai_output_schemas.js; routes/chat.js; public/lbc-chat-drawer.js; services/ai_model_config.js; services/ai_gateway.js. Private prompt text and API credentials are not published.

**Verification limit:** These are source-evidenced behaviors; actual customer results depend on data, configured AI providers, permissions and the running deployment. Competitor similarity is based on published product materials, not access to their private implementations.

[Full feature register](FEATURE-MATRIX.md) · [Five-competitor comparison](COMPARISON.md) · [Live product](https://lockeprofessional.com/) · [Video](https://lockeprofessional.com/guided-demo/locke-professional-demo.mp4)