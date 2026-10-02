# Modern SEO — Foundation and Validation Notes

> **Scope and source status.** This is a concise working-note capture of the accessible written companion material in the **Modern SEO** classroom of *AI SEO Mastery with Caleb Ulku*, reviewed on **2026-10-01**. It adds material that was not represented as a standalone source in the repository as of commit `2e4ad84` (2026-08-26). It does **not** reproduce course videos or promise rankings.
>
> **Evidence labels used below**
>
> - **Course-confirmed** — the lesson’s written companion states or recommends it.
> - **First-party verified** — Google’s own documentation supports the statement.
> - **Practical heuristic** — a course workflow, measurement threshold, timing estimate, or implementation choice. Treat it as a testable operating hypothesis, **not** a Google ranking rule.
>
> **Deliberate separation:** Google Business Profile (GBP) work and **Website SEO** work are related, but this document tracks them in separate lanes. Do not turn a website audit into unapproved GBP edits, or vice versa.

## What is newly captured

The repository already documented the Prompt Catalog and the separate Core 30 build course. The net-new material here is the classroom’s **Modern SEO** foundation: a diagnostic sequence, the low-competition three-step workflow, validation controls, and an explicit measurement/escalation model.

| Classroom section reviewed | Written lessons inventoried | Repository treatment |
|---|---|---|
| **The Local SEO Reality Check** | Modern SEO Welcome; Live Website Breakdown; How Google and AI Actually Work; How We Do Local SEO; The Low Competition Ranking Method | New source capture; distilled below. |
| **Complete Low-Competition Ranking Method** | Complete GBP Audit and Optimization; GBP Landing Page Audit and Optimization; Citations and Trust Signals that Work; Putting It All Together | New source capture; distilled below. |
| **Core 30 System Introduction** | What the Core 30 Framework Is; Core 30 Gap Analysis; Single Prompt Content Creation | Inventory confirmed. Detailed build methodology remains in `Core_30_Website_Build_Course_Notes.md` and `Core_30_Agent_and_Operations_Playbook.md`; not duplicated here. |
| **Client Acquisition Fundamentals** | Facebook Ads Overview + Unlock; Local Business Networking Strategies; YouTube / Content Marketing; Pricing Framework; What Happens When You Outgrow Modern SEO | Inventory confirmed. Existing operations and pricing notes remain the repository’s working reference; this capture stays focused on SEO foundation and validation. |

## 1. The useful new operating model

### 1.1 Start with a documented baseline

**Course-confirmed.** The Modern SEO method begins by recording a local rank-map baseline before optimization, then checking it every two weeks. It uses the trend to decide whether to stay with foundational work or investigate a more comprehensive content/architecture approach.

**Recommended operationalization.** Capture the baseline before a material change and attach the date, tested query set, grid configuration, device/location settings, current GBP state, and website state. Pair map visibility with outcome metrics such as calls, qualified leads, Search Console performance, and on-site conversion behavior. A rank-map color percentage by itself is not a business outcome or a Google metric.

**Google-aligned guardrail.** Google says local results are mainly based on **relevance, distance, and prominence**, and says there is no way to request or pay for better local ranking. Google does not publish a universal “green coverage” target. [1]

### 1.2 Diagnose before changing

**Course-confirmed.** The classroom’s diagnostic lesson emphasizes a repeatable order: identify the business’s primary category and services; inspect the GBP-connected landing page; review title/H1 and local-business schema; compare business facts; and prioritize the largest, evidenced gaps before advanced tactics.

**Recommended diagnostic record**

| Order | Google Business Profile lane | Website SEO lane | Evidence to save |
|---|---|---|---|
| 1 | Record current primary/additional categories, services, address/service-area model, hours, and profile link. | Record canonical landing-page URL, status, indexability, title, H1, phone/address display, schema, and key conversion elements. | Dated screenshots; export/notes; URL Inspection and Search Console evidence where available. |
| 2 | Verify the facts represent the real business and record any existing ranking/verification risk before proposing edits. | Test the page as Google can access it; review crawl/indexing status before treating an on-page idea as a ranking fix. | Business-source proof, live URL test, schema test, source HTML where needed. |
| 3 | Identify only accurate, meaningful profile gaps. | Identify only evidence-backed site gaps: broken rendering, wrong facts, missing unique content, weak intent match, unclear titles, or schema errors. | A before-state checklist with owner, risk, and expected user benefit. |
| 4 | Draft profile changes separately for approval. | Draft website changes separately for approval. | Change log and explicit approval record. |
| 5 | Measure after implementation; do not repeatedly toggle settings without evidence. | Measure crawling, indexability, Search Console, and business outcomes after a reasonable processing period. | Dated post-change comparison. |

## 2. Google Business Profile lane — course workflow with policy guardrails

### 2.1 Course-derived GBP audit sequence

**Course-confirmed.** The course’s audit sequence is: review the current primary category; check existing visibility before considering a primary-category change; evaluate accurate secondary categories; inventory current and missing real services; verify information; and document the before/after state. It repeatedly cautions against unnecessary changes to an already-performing primary category.

**First-party verified constraints.** Google says to select a primary category that best describes the business, choose a specific category from Google’s list when possible, and add another category only from that list. Google’s representation guidelines say to use the **fewest number of categories** needed to describe the core business, accurately represent the business, and keep the address/service area precise. Editing an existing category can trigger re-verification. [2] [3]

**Practical controls**

- Never add a category or service merely because it has search volume. Confirm the business actually provides it and can substantiate the claim.
- Treat a primary-category change as a controlled experiment: document existing visibility and reason for the proposal, notify the owner of possible verification/volatility, and obtain approval before editing.
- Keep GBP changes separate from website changes. A change request should name its lane, owner, source of truth, expected user benefit, and rollback path.
- Verify the profile is claimed/managed by the authorized business representative before proposing administrative changes.

### 2.2 What Google supports—and what it does not promise

Google states that complete, accurate Profile information can help a business appear for relevant local searches and that positive reviews and helpful replies can help a business stand out. It identifies relevance, distance, and prominence as the principal local-result factors. [1]

Google does **not** say that a particular category count, specific service wording, citation vendor, map-grid percentage, or title-tag pattern guarantees a rank improvement. The course’s workflow is therefore useful as a structured audit method, but its predicted outcomes must remain hypotheses.

## 3. Website SEO lane — GBP landing-page validation

### 3.1 Course-derived checklist

**Course-confirmed.** The Modern SEO landing-page lesson checks the page selected on the GBP—often the homepage—for:

1. A public, usable landing page that accurately represents the business;
2. LocalBusiness structured data that matches the visible business facts;
3. Consistent visible phone and address information across key templates/pages;
4. A clear, truthful title and H1 aligned to the page’s real service/location purpose;
5. A documented before/after state and a validation step after implementation.

### 3.2 Google-aligned implementation standards

- Google’s LocalBusiness structured-data documentation says structured data can communicate business information to Google; it recommends using the most specific applicable subtype, defines `name` and `address` as required properties for LocalBusiness eligibility, and advises validating code with the Rich Results Test before testing the deployed page in URL Inspection. [4]
- Structured data must accurately represent the page and comply with Search Essentials and Google’s general structured-data policies. Valid markup is not a guarantee of a rich result or a ranking change. [4]
- Google’s SEO Starter Guide supports clear, unique, concise titles that accurately describe the page. It does not prescribe one fixed title formula or character threshold as a ranking formula. [5]
- Use source-of-truth business facts. If public business information is intentionally formatted differently in a specific context, document why; do not change information blindly solely to create a punctuation match.
- A map/GBP embed may be a useful visitor convenience on a location page, but the classroom’s claim that it is a decisive ranking signal is **not presented here as a Google-confirmed fact**.

### 3.3 Website SEO pre-change control

Before implementation, confirm that the planned URL is the intended canonical page, is accessible to visitors and Google, does not carry accidental `noindex`, renders key content, and has a clear searcher purpose. Use Search Console evidence and URL Inspection rather than treating schema, headings, or local wording as a substitute for basic indexability and useful content. [5]

## 4. Citations and local trust — practical, not a shortcut

**Course-confirmed.** The classroom differentiates verified listings on major maps/directories from indiscriminate directory submissions. Its recommended process is to distribute only accurate source data, inspect the resulting listings, correct errors, and maintain important profiles.

**Recommended operationalization.** Maintain a citation ledger with platform, URL, claim/verification status, NAP/service/hours source, last verified date, and correction owner. Prioritize customer-facing, authoritative platforms that are relevant to the business and market. Do not create duplicate profiles, invent services, use virtual addresses, or submit inconsistent information.

**What remains a hypothesis.** The course uses proprietary terminology (“super citations”) and describes a vendor-specific distribution network and predicted trust/ranking effects. Those vendor claims, exact platform counts, processing times, and comparative effectiveness have not been independently verified in this repository. They are not Google policy and should not be used as a reason to bypass a platform’s normal verification rules.

## 5. Measurement and escalation model

### 5.1 Course heuristic

The course proposes a phased, two-week review cadence: implement the foundation; allow time for processing; assess the rank-map trend; and consider a larger Core 30 content/architecture project only if foundational work is not producing adequate progress in a sufficiently long observation period.

### 5.2 SEO Mastery measurement standard

Use the course phases as an **experiment framework**, not an automatic rule:

| Stage | Required evidence | Decision rule |
|---|---|---|
| **Baseline** | Rank-map configuration, GBP facts, Search Console query/page/device data, indexed/canonical landing page, lead baseline. | No implementation decision without a documented starting point. |
| **Foundational corrections** | Approved GBP and/or website change log, validation results, sitemap/indexing state if applicable. | Fix demonstrated quality, consistency, technical, or user-value gaps first. |
| **Observation** | Date-bounded performance comparison; Search Console trends; GBP Performance data where available; leads/calls; rank-map trend. | Avoid declaring success/failure based on a few days or a single location/query. |
| **Escalation** | Evidence that important services/intent are not represented by clear, unique pages; competitor/SERP review; indexability and quality checks. | Consider Core 30 only when the business case and the evidence support a distinct page architecture—not because a generic threshold was missed. |
| **Reassessment** | Change log plus incremental results and unresolved hypotheses. | Preserve what is working; test the next smallest meaningful improvement. |

Google’s SEO Starter Guide advises allowing time for changes to be reflected and evaluating outcomes rather than assuming a visible performance effect. [5]

## 6. Claims to treat as hypotheses—not doctrine

| Course claim or shortcut | SEO Mastery handling |
|---|---|
| A specific three-step sequence works for “70–80%” of businesses. | Use as a course framing statement only; no independent validation is recorded here. |
| A city-population cutoff distinguishes easy and difficult markets. | Treat local competition as query-, service-, location-, and competitor-specific. Validate with evidence. |
| A rank-map percentage (for example, 30–40% green) dictates the next tactic. | Use the trend as a planning input, alongside leads, SERP changes, business goals, and Search Console data. |
| Exact public phone/address punctuation determines rankings. | Maintain accurate, comprehensible, source-controlled business information; do not elevate formatting minutiae into an unproven ranking rule. |
| A GBP embed is a decisive local-ranking signal. | Evaluate it primarily as a visitor/convenience feature unless evidence shows another clear benefit. |
| A citation service or fixed number of listings creates a particular rank result. | Vet service terms, data accuracy, duplicate-profile risk, privacy, verification method, recurring cost, and measurable results before purchase or rollout. |
| ChatGPT recommendations require a particular Bing profile. | Do not treat as established platform behavior without current first-party documentation and independent testing. |

## 7. Crowley’s Granite & Quartz application boundary

This knowledge capture does **not** change Crowley’s website, Google Business Profile, Search Console, schema, citations, or tracking. For Crowley’s work, retain the project’s Google-first diagnostic order:

1. **Website SEO:** Search Essentials → Search Console evidence → SEO Starter Guide → Status Dashboard only for broad anomalies → documented escalation if unresolved.
2. **Google Business Profile:** Separate factual/profile audit → evidence-backed proposal → explicit approval before edits → record changes and measure after implementation.
3. **Content/architecture:** Propose a distinct page only when a real user need, intent, and original local evidence justify it; avoid interchangeable location pages and keyword stuffing.

## 8. Lesson links reviewed

1. [Modern SEO Welcome](https://www.skool.com/ai-seo-mastery/classroom/78805191?md=dc4f782583d14b79b996b0e60ee82be0)
2. [Live Website Breakdown](https://www.skool.com/ai-seo-mastery/classroom/78805191?md=3eb3e95398e140b5b5536f8b6c463fc4)
3. [How Google and AI Actually Work](https://www.skool.com/ai-seo-mastery/classroom/78805191?md=be9f77faa3c1413b90570f99166314c6)
4. [How We Do Local SEO](https://www.skool.com/ai-seo-mastery/classroom/78805191?md=22e50b2d77c1465cbf0a78821ef16bcf)
5. [The Low Competition Ranking Method](https://www.skool.com/ai-seo-mastery/classroom/78805191?md=aaf4c27d3d8b452db2e2e35ae6b37129)
6. [Complete GBP Audit and Optimization](https://www.skool.com/ai-seo-mastery/classroom/78805191?md=c2e6552cad0040849810dab27bb8eb74)
7. [GBP Landing Page Audit and Optimization](https://www.skool.com/ai-seo-mastery/classroom/78805191?md=8ed70da8f1c14165b73f83f9e044a275)
8. [Citations and Trust Signals that Work](https://www.skool.com/ai-seo-mastery/classroom/78805191?md=fa952280b3b94b27894c568f5d0c7ecb)
9. [Putting It All Together](https://www.skool.com/ai-seo-mastery/classroom/78805191?md=2ccef1e3baa74542864c2527873e3532)

## References

[1]: https://support.google.com/business/answer/7091?hl=en "Google Business Profile Help — Tips to improve your local ranking on Google"
[2]: https://support.google.com/business/answer/7249669?hl=en "Google Business Profile Help — Manage your business category"
[3]: https://support.google.com/business/answer/3038177?hl=en "Google Business Profile Help — Guidelines for representing your business on Google"
[4]: https://developers.google.com/search/docs/appearance/structured-data/local-business "Google Search Central — LocalBusiness structured data"
[5]: https://developers.google.com/search/docs/fundamentals/seo-starter-guide?hl=en "Google Search Central — SEO Starter Guide"
