# Core 30 Agent and Local SEO Operations Playbook

**Status:** Draft knowledge-base addition, compiled from the AI SEO Mastery course notes, the accessible Prompt Catalog, a supplied interview transcript, and current first-party platform documentation.  
**Purpose:** Convert the Core 30 methodology into an operational system for planning, production, quality control, delivery, pricing, and measurement.

> **Source discipline:** This playbook distinguishes between **course-confirmed method**, **first-party platform guidance**, and **interview-derived agency practice**. Interview-derived workflows are useful implementation patterns, not verified Google or OpenAI policy.

## 1. Operating Model

Local SEO is the systematic work of making a legitimate business easier for search and answer systems to understand, trust, retrieve, and recommend for a relevant local need. For Google local results, the documented foundation is **relevance, distance, and prominence**. Complete business information supports relevance; distance reflects the searcher’s or inferred location; and prominence includes signals such as public links and reviews. [1]

The Core 30 is the website-side structure that reinforces the Google Business Profile (GBP). It maps each real GBP category and service into a coherent page, URL, and internal-link system. The result is not a collection of generic pages. It is an intelligible hierarchy that connects the **business**, its **categories**, its **services**, and its **service area**.

| Layer | Primary question | Core artifact |
|---|---|---|
| Business entity | Who is the business, and can its identity be trusted? | Accurate GBP, NAP, reviews, citations, real About evidence, schema |
| Service entity | What does the business actually do? | GBP services, category/service pages, service schema, exact service naming |
| Geographic entity | Where is the business relevant and competitive? | GBP location/service area, rank grid, local evidence, location content when justified |
| Conversion layer | Why should a ready-to-buy visitor call or inquire now? | GBP landing page, proof, reviews, differentiators, lead form, phone CTA |
| Technical layer | Can systems crawl, interpret, and use the information? | Rendered HTML, metadata, schema, sitemaps, robots, canonical URLs, performance |

## 2. Core 30 Build Workflow

The following sequence consolidates the Core 30 course workflow. The numbered prompts are documented separately in `Core_30_Website_Build_Course_Notes.md`; this section describes how they operate as a delivery system.

| Stage | Required work | Primary output | Quality gate |
|---|---|---|---|
| 1. Intake and research | Confirm NAP, GBP categories, services, service areas, competitors, proof points, reviews, licensing, hours, images, and conversion goals. | Verified business facts and normalized service inventory. | Do not invent trust signals, service claims, or availability. |
| 2. Architecture | Build the source-of-truth hierarchy: homepage, secondary categories, core-service hubs, child services, general services, About, Contact, and planned location/supporting content. | Prompt 0 architecture block, URL map, linking map, and page-count summary. | Every real service belongs to one logical parent; no orphan page types. |
| 3. Skeleton | Create routes, global header/footer, mobile navigation, call actions, `/services` hub, and `ScrollToTop` behavior. | Complete routable site shell. | No placeholder page should be exposed to indexing before substantive content is ready. |
| 4. GBP landing page | Write conversion copy from real differentiators, then implement it with proof, reviews, lead capture, primary service paths, and calls to action. | Homepage/GBP landing page. | Lead with the visitor’s problem and proof, not company history or generic slogans. |
| 5. Category and core-service hubs | Build authoritative parent pages that explain the category/core service, link to every relevant child service, and point back to the homepage. | Secondary-category and core-service hub pages. | Use correct internal hierarchy and locally accurate content. |
| 6. Child-service pages and `/services` | Build a useful page for every actual service and a complete services directory. | Child-service pages plus service navigation hub. | Each child page links back to the correct parent. |
| 7. About and Contact | Add verifiable human/business evidence and simple lead paths. | Authentic About and functional Contact page. | Real people, photos, credentials, and contact handling—not fabricated E-E-A-T. |
| 8. Technical SEO | Verify rendering, indexability, sitemap, robots, schema, metadata, links, mobile usability, page speed, canonicals, Open Graph, and 404 behavior. | Technical launch and audit report. | Validate actual rendered output and live routes, not only code intent. |
| 9. Geographic expansion | Use rank-grid evidence to choose priority areas, then create only genuinely differentiated, research-supported location content. | Ranked geographic opportunity queue and evidence-led location pages. | Positions 4–6 are first-priority opportunities; do not mass-produce near-duplicate city pages. |
| 10. Measurement and iteration | Compare baseline with current rank grid, indexing, GBP visibility, qualified calls/forms, traffic, and page-cluster performance. | Monthly client report and next-sprint plan. | State what changed, what was done, what was learned, and what happens next. |

## 3. GBP and Conversion-Led Landing Pages

The GBP landing page is the highest-stakes conversion page in the Core 30 system. Its function is to help a visitor with an immediate local need decide whether to call, request a quote, or take the next qualified step. The course therefore separates homepage **content creation** from **implementation** rather than asking one generic prompt to create a finished page in a single pass.

The page should begin with the local service outcome, a visible call-to-action, and credible proof. The recommended sequence is: hero, real differentiators, visible review/social proof, lead capture, service paths, compact coverage information, credentials, FAQs, and a final CTA. The business history belongs lower on the page or on the About page unless it is directly relevant to the customer’s immediate decision.

| Conversion input | Acceptable evidence | Avoid |
|---|---|---|
| Review proof | Accurate count/rating, embedded or linked review source, permitted testimonial | Invented reviews or unverified star counts |
| Response/process claim | Documented hours, quoted process, dispatch or scheduling policy | “Same day,” “24/7,” or response times that are not true |
| Licensing and credentials | Actual license/certification and scope | Generic “licensed and insured” presented as the sole differentiator |
| Ownership and experience | Verifiable local ownership, years, team expertise | Long company-history narrative above the conversion content |
| Service proof | Project photos, material/process explanations, case studies, relevant warranties | Stock claims, generic “quality service,” or unrelated blog filler |

## 4. Geographic Relevance: From Rank Grid to Evidence-Led Pages

The course’s Geographic Content Gap Finder uses local rank-grid data to identify opportunity neighborhoods. Areas ranking in positions **4–6** are “striking distance” opportunities and should generally receive priority before areas ranking 7 or worse. [2]

The interview-derived extension is a production standard for location content. A location page should be substantively different because the business context is different, not because a city or landmark name has been swapped.

### Research standard

Before drafting a location-oriented page, assemble a compact evidence packet appropriate to the business and area. Possible source types include official local data, local regulations, public infrastructure information, map/distance information, search results, local discussion sources, relevant property or neighborhood context, the business’s real service history, and verified review language. Use only details that are relevant, lawful to use, and capable of verification.

### Drafting standard

Use the evidence packet to explain the service problem, customer/property context, access or logistics considerations, local terminology, and service path. Do not assert hyperlocal facts merely to sound local. If a source cannot support a claim, remove or soften it.

### Similarity-control standard

Before publishing, compare candidate pages against nearby location pages. Reject text that could be made interchangeable by replacing the location name. Distinct content should be anchored in different customer needs, building stock, local conditions, commercial/residential context, service constraints, landmarks, or documented evidence.

> **Important:** The interview’s description of an April 2026 de-indexing event and an “informationally additive” test is retained only as an agency observation. Google’s public ranking-update history does not list an April 2026 ranking update. [3]

## 5. Core 30 Agent: Operating Specification

The **Core 30 Agent** is an interview-derived agency tool concept, not a documented classroom product. Its purpose is to reduce repetitive research, drafting, checking, and production work while preserving factual discipline and human approval.

| Component | Responsibilities | Human control point |
|---|---|---|
| Intake normalizer | Validates business identity, GBP categories, services, service areas, contact data, assets, and proof. | Approve factual business profile before drafting. |
| Architecture engine | Produces page map, hierarchy, URL plan, internal-link graph, and page count from the verified service inventory. | Review categories, parent/child assignments, and high-value service hubs. |
| Rank-grid analyzer | Finds weak areas, position 4–6 clusters, position 7+ growth areas, and geographic opportunity priority. | Confirm that opportunity areas are commercially sensible and actually served. |
| Evidence collector | Builds source packets for services, geography, reviews, proof, and content context. | Validate sources, dates, claims, and permission-sensitive material. |
| Content planner | Produces page briefs, outlines, differentiation requirements, internal-link targets, and conversion objectives. | Approve page strategy before generating long-form content. |
| Drafting engine | Creates first drafts from the approved brief and evidence packet. | Require editorial review for facts, voice, claims, pricing, and real-person material. |
| QA engine | Checks duplication, unsupported claims, hierarchy, page length, schema inputs, metadata, links, forbidden phrasing, and conversion elements. | Review failed checks and approve exceptions. |
| Publishing and reporting layer | Queues approved content, tracks implementation, and produces baseline/current/next-sprint reporting. | Confirm publication and client-facing reports. |

### Multi-pass content protocol

The interview mentions an eight-pass Claude Sonnet process supported by multiple data calls, but it does not specify the eight pass names. The following is a **recommended operationalization**, not a claim about the original system:

| Pass | Objective |
|---|---|
| 1. Fact intake | Normalize and deduplicate only verified business facts. |
| 2. Opportunity selection | Select a page target from the architecture, rank grid, or commercial priority. |
| 3. Evidence assembly | Build a source packet and flag unverifiable gaps. |
| 4. Brief and outline | Define user intent, information gain, conversion objective, link targets, and section plan. |
| 5. Draft | Write from the brief and evidence packet, not from a generic city/service instruction. |
| 6. Claim and duplication audit | Remove unsupported claims and compare against related pages. |
| 7. Technical/content QA | Check metadata, headings, internal links, schema inputs, readability, and mobile conversion elements. |
| 8. Human approval | Approve, revise, or reject prior to publishing. |

## 6. Human-AI Governance

AI can accelerate structured research, analysis, outlining, and first-draft production. It should not be allowed to invent factual business claims, impersonate real people, publish unreviewed sensitive communications, or replace editorial judgment where brand reputation is at stake.

| Content type | Recommended production mode |
|---|---|
| Service, category, and research-supported geographic pages | AI-assisted research/drafting with source validation and human approval. |
| GBP landing page | Human-led conversion strategy; AI may assist paragraph by paragraph, but proof, positioning, and final copy require review. |
| About page, owner biographies, credentials, licenses, project stories | Human-provided facts and assets; AI may edit, but not invent. |
| Customer newsletters, founder posts, sales outreach, public thought leadership | Human-authored or closely human-edited. Preserve authentic voice and accountability. |
| Technical implementation | AI-assisted development is acceptable only with tests, peer/model critique where useful, and human approval before deployment. |

### Multi-model author/critic workflow

The interview describes an engineering workflow in which several models independently diagnose a problem, agree on a proposed fix, then fresh critic instances assess that fix before a human reviews it. That is a useful pattern for nontrivial automation and code changes.

The operational rule is simple: **use model agreement as a quality signal, not as a substitute for testing or accountable review.** Every release still requires tests, rollback awareness, security review where applicable, and a human decision.

## 7. Pricing and Scope Framework

> **Commercial note:** This is a draft operational framework, not financial advice or a mandated rate card. Validate pricing against labor time, subcontractor cost, tool cost, client risk, market competition, and margin before quoting. The interview mentions historical $2,000–$3,000 monthly examples, but those anecdotes are not recommended current prices.

The preferred model is **transparent scope-based pricing**, not a black-box promise to “get rankings.” Quote the work, the throughput, the responsibilities, and the measurement plan. Do not guarantee a ranking position or fixed result by a deadline.

| Tier | Use case | Typical scope | Pricing unit |
|---|---|---|---|
| 0. Diagnostic and architecture | New engagement, audit, rescue, or pre-build planning | GBP/service audit, competitor/context review, rank baseline, service inventory, Core 30 architecture, roadmap | One-time fixed discovery/strategy fee |
| 1. Foundation | Business has a viable site but weak entity, conversion, or technical basics | GBP cleanup, NAP/citation corrections, key landing-page upgrade, technical fixes, first priority service/category pages | One-time implementation package plus optional support retainer |
| 2. Core 30 build | Business needs a complete category/service architecture | Full site map, routes/templates, homepage, category/core/child service pages, About/Contact, schema, technical launch work | Fixed build scope priced by approved page count and complexity |
| 3. Geographic growth | Business has a working Core 30 and needs selective coverage expansion | Rank-grid review, evidence packets, differentiated location/supporting content, internal links, performance monitoring | Monthly or sprint-based price per approved research/content cluster |
| 4. Authority and conversion optimization | Established business needs durable gains and higher lead quality | Review strategy, citations/authority, digital PR/link work, CRO experiments, project evidence, reporting | Monthly retainer tied to deliverable quantity and program complexity |
| 5. Agent-enabled managed SEO | Mature workflow with automation and editorial controls | Ongoing research, production, QA, implementation coordination, reporting, human review | Monthly managed-service fee, transparently tied to throughput, review level, and tooling |

### Scope estimator

A defensible quote should include a one-time setup component, a delivery component, and an ongoing governance component.

| Cost driver | How to define it |
|---|---|
| Architecture complexity | Number of categories, core-service hubs, child services, general services, and required templates. |
| Content effort | Number of pages, word/section requirements, research depth, visual needs, legal/claim sensitivity, and editorial review. |
| Geographic complexity | Number of priority neighborhoods, competitive intensity, rank-grid gaps, source-collection time, and differentiation burden. |
| Technical effort | CMS/Lovable/custom-code constraints, rendering solution, migrations, form integrations, schema, analytics, and QA. |
| Authority effort | Citation cleanup, linkable assets, outreach, reputation work, review generation policy, and local partnerships. |
| Reporting and governance | Meeting cadence, dashboard/report depth, stakeholder count, client approvals, and change-management overhead. |

### Commercial rules

The scope document should say what will be done, why it matters, how success will be measured, what the client must supply, and what is excluded. Avoid fixed ranking guarantees. A useful monthly report contains a baseline/current comparison, completed work, indexing/technical findings, conversion signals, what was learned, and the next approved sprint.

## 8. Measurement and Reporting

Measure the work as a system. The map pack, organic pages, Business Profile, phone calls, quote forms, and indexation can move differently. Use a consistent baseline and compare like with like.

| Measurement layer | Primary checks |
|---|---|
| Rank grid | Positions by coordinate, priority 4–6 clusters, map visibility trend, service/category query coverage. |
| Search and indexation | Indexed pages, excluded/noindex/duplicate states, impressions, clicks, query groups, and crawl/rendering issues. |
| GBP | Profile completeness, categories/services, reviews/replies, calls, directions, website actions, photos, and conversion actions available in the profile. |
| Website conversion | Call clicks, form starts/submits, quote requests, phone quality, landing-page behavior, and source attribution. |
| Content quality | Duplicate/near-duplicate patterns, source-backed claims, internal links, heading hierarchy, local specificity, and current proof. |
| Technical SEO | Live rendered HTML, canonical URLs, metadata, schema validity, sitemap/robots, performance, mobile usability, 404 behavior, and broken/orphan links. |

## 9. Platform Guidance and Guardrails

The interview contains useful models, but the following points should be applied with accuracy:

| Topic | Operating rule |
|---|---|
| Keywords and entities | Do not keyword-stuff. Use natural exact language where it clarifies the service and location. Google still identifies matching query terms as a basic relevance signal while also using language understanding and related terms. [4] |
| Links and authority | Earn relevant, legitimate references and citations. Links are meaningful prominence/quality signals, but they are not the only ranking factor. [1] [4] |
| Local ranking | Treat relevance, distance, and prominence as the documented Google local-search foundation. Do not promise that content can overcome every distance or competition constraint. [1] |
| ChatGPT visibility | Maintain accessible, accurate websites and strong business information across relevant sources. ChatGPT Search uses third-party providers, including Bing and Shopify, and uses approximate or optional precise location for local results. Do not assume a single listing controls visibility. [5] |
| Google update claims | Record agency observations, but distinguish them from official updates. Google’s public history listed March and May 2026 updates, not an April 2026 ranking update. [3] |
| Generic blogs | Do not publish filler. Retain or create educational/supporting content only when it serves a real query, strengthens an important service theme, provides distinct information, or contributes to conversion/authority. |

## 10. Recommended Knowledge-Base Maintenance

The repository should retain prompt-level notes separately from operating playbooks. Update this document when new interviews, tool workflows, or validated platform guidance change the practical process.

| Document | Purpose |
|---|---|
| `Core_30_Website_Build_Course_Notes.md` | Canonical capture of the numbered Core 30 course workflow. |
| `Prompt_Catalog_Notes.md` | Catalog of classroom prompts and workflows beyond the build sequence. |
| `Core_30_Agent_and_Operations_Playbook.md` | Operational system: evidence-led geography, agent design, human-AI governance, scope/pricing, reporting, and platform guardrails. |
| `README.md` | Repository map, provenance, and guidance on how to use each document. |

## References

[1]: https://support.google.com/business/answer/7091?hl=en "Google Business Profile: Tips to improve your local ranking on Google"
[2]: https://www.skool.com/ai-seo-mastery/classroom/31982aaa?md=d975f5c22f6847e3b2f2f1dc2b01d9b7 "AI SEO Mastery: Geographic Content Gap Finder"
[3]: https://status.search.google.com/products/rGHU1u87FJnkP6W2GwMi/history "Google Search Status Dashboard: Ranking update history"
[4]: https://www.google.com/intl/en_us/search/howsearchworks/how-search-works/ranking-results "Google: How Search ranking works"
[5]: https://help.openai.com/articles/9237897-chatgpt-search "OpenAI: ChatGPT Search"

## Internal Source Notes

This playbook also draws from Dan’s supplied interview transcript, which contains agency-reported workflows and observations. Those elements have been labeled as interview-derived and separated from course-confirmed or first-party platform information.
