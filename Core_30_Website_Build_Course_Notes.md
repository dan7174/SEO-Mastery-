# Build a Core 30 Website with AI — Course Notes

*Course by Caleb Ulku (AI SEO Mastery) — organized reference document*
*Companion to **AI SEO Mastery — Complete Class Notes**. Separate document covering the website-build sequence only. Cross-references point back to the main notes.*

**Status:** ✅ The **Overview**, all 9 prompts (0–8), and the **Lovable HTML** lesson have been captured and cross-referenced.

**Build environment:** This course builds sites in **Lovable** (AI app/site builder). Worked example throughout is a plumber in Gary, IN ("Gary Plumbing Company" → `ai-seo-pro-gary.lovable.app/plumber-gary-in`).

**Structure note:** The course is **Prompt 0 → Prompt 8 (nine prompts)** plus two non-prompt framing lessons (Overview, Lovable HTML). The "8 prompts" shorthand refers to the eight build prompts (1–8); Prompt 0 is planning/setup.

---

## How this document works

Same analytical approach as the main notes. For each lesson I'll capture:
- The verbatim prompt (blockquoted)
- What it does / what it outputs
- Usage notes (inputs required, customization, gotchas)
- 🔄 **Cross-references & overlaps** — where this duplicates or extends something already in the main notes
- Its role in the end-to-end build sequence

**Flag legend** (matches main notes):
- ✅ Confirmed duplicate of existing documented material
- 🔄 Partial overlap / extends an existing prompt
- ⭐ Pivotal / master prompt in the sequence
- ⚠️ Caveat, risk, or decision point
- 🆕 Net-new material not present anywhere in the main notes

---

## Table of Contents

0. [Overview (framing lesson)](#overview-framing-lesson)
1. [Prompt 0 — Planning](#prompt-0--planning)
2. [Lovable HTML: NEEDED to Get Ranked (framing lesson)](#lovable-html-needed-to-get-ranked-framing-lesson)
3. [Prompt 1 — Skeleton](#prompt-1--skeleton)
4. [Prompt 2 — GBP Landing Page Content](#prompt-2--gbp-landing-page-content)
5. [Prompt 3 — GBP Landing Page Build Out](#prompt-3--gbp-landing-page-build-out)
6. [Prompt 4 — Secondary Category Page Build Out](#prompt-4--secondary-category-page-build-out)
7. [Prompt 5 — Core Service Page Build Out](#prompt-5--core-service-page-build-out)
8. [Prompt 6 — Service Page Build Out](#prompt-6--service-page-build-out)
9. [Prompt 7 — About and Contact Page Build Out](#prompt-7--about-and-contact-page-build-out)
10. [Prompt 8 — Technical SEO Implementation](#prompt-8--technical-seo-implementation)
11. [Cross-Reference Map (running)](#cross-reference-map-running)
12. [Workflow Logic — The Build Sequence](#workflow-logic--the-build-sequence)
13. [Open Questions / To Verify](#open-questions--to-verify)
14. [References](#references)

---

# Overview (framing lesson)

**Runtime:** ~7:07 (video) — *not a prompt.*

**What it covers:**

The lesson tours the finished **Core 30 sample site** for a plumbing business in Gary, Indiana. It establishes the course’s intended end state: a simple-looking local-service website with roughly **60 pages**, organized around category pages, high-priority service hubs, child-service pages, a services hub, and a locations hub.[1]

> The Overview’s main message is that the build is not merely a collection of pages. Its title tags, H1s, conversion copy, page hierarchy, and internal links are designed to reinforce one another.

| Topic | Course guidance captured from the Overview |
|---|---|
| **Search-result targeting** | The title tag should prominently include the **primary GBP category and city**. The H1 should repeat that core relevance signal while adding a clear, compelling reason to call. |
| **Goal completion** | The visitor should immediately see why the business is the right choice and why they should call or convert. The walkthrough uses proof, review visibility, and direct problem-solving before educational detail. |
| **Homepage linking priority** | The homepage links to secondary-category pages and to selected, high-priority service hubs. In the plumbing example, water-heater replacement and main-drain-line replacement are elevated because they are services the business especially wants to rank for. |
| **Service-hub logic** | A high-value service can function as a hub even when it is not a GBP category. The hub then links to its related child-service pages. |
| **Services hub** | The `/services` page serves as the complete, prioritized directory of category services, core-service hubs, and additional general services that are not all linked directly from the homepage. |
| **Geographic relevance** | The example includes a locations hub. The lesson directs learners to use the separate geographic-relevance method: examine the local rank map, identify weaker areas (for example, locations showing positions 4–6), and create content that combines the target category or service with a relevant landmark and city. |
| **Build workflow** | Prompt 0 is completed before entering Lovable; its architecture output is pasted into every later prompt. Prompt 1 builds the skeleton. Prompt 2 pre-writes GBP landing-page content, which Prompt 3 then implements in Lovable. |
| **Copy-quality control** | The instructor explicitly warns against allowing Lovable to generate low-quality copy and publish it unchanged. For client work, the more rigorous course copywriting process can be used for every important page type, not only the homepage. |
| **Crawlability dependency** | The Overview previews a separate Lovable HTML lesson because Lovable sites can have a search-visibility problem if Google cannot see the rendered content. That lesson is therefore a rank-readiness dependency, not an optional afterthought. |

**Practical implementation notes:**

- The demo’s locations hub confirms that location content belongs in a complete Core 30 site; however, this course’s numbered prompts do **not** contain a dedicated location-page generator. The location-content method belongs to the separate geographic-relevance material. Treat the `/locations/` links in Prompt 3 as conditional until that content has been built.
- The course uses a split workflow intentionally: **architecture first**, then **site scaffold**, then **pre-written content for the highest-stakes page**, then implementation. The instructor notes that the same pre-writing discipline can be extended to secondary-category, core-service, service, about, and contact pages when quality matters.
- The sample footer remains deliberately minimal: NAP information, logo, repeated navigation, privacy policy, and terms. Keep the current-year value accurate before launch.

🔄 **Cross-references & overlaps:**
- Live demo site (`ai-seo-pro-gary.lovable.app/plumber-gary-in`) is the end-state this whole sequence produces. Compare the finished page against the **Homepage (GBP Landing Page)** spec in *The Complete Playbook* and the *AI Agent Prompt — Local Business Website Builder*.
- The walkthrough validates the hierarchy later formalized in Prompts 0, 5, and 6: **secondary category → child services**, **core service hub → child services**, and **general services → services hub/homepage**.
- The Overview explains the rationale behind the Prompt 2 → Prompt 3 handoff: write critical conversion content first, then instruct Lovable to build the page from that approved content.
- The locations hub is an important scope distinction: it appears in the finished example, but its creation relies on the course’s separate **Building Geographical Relevance** process rather than the numbered Core 30 build prompts.

---

# Prompt 0 — Planning

**Role assigned:** "Local SEO expert who specializes in site architecture for service businesses."

**The prompt:**

```
You are a local SEO expert who specializes in site architecture for service businesses. Your task: help me plan the complete site structure for a local business website before we build it. This structure will be used to create all pages, navigation, and internal linking.

BUSINESS INFORMATION — TELL ME ABOUT YOUR BUSINESS
BUSINESS NAME / INDUSTRY / CITY / STATE / STATE ABBREVIATION / ZIP CODE / PHONE / EMAIL
PRIMARY GBP CATEGORY / SECONDARY GBP CATEGORIES (if any)
SERVICES YOU OFFER (list ALL — be comprehensive)
SERVICE AREAS (all cities/neighborhoods served)

YOUR TASK — create a complete site architecture that includes:
1. URL STRUCTURE — homepage = /[primary-category-slug]-[city-slug]-[state-abbrev]; all pages follow same pattern
2. SERVICE HIERARCHY — Secondary Categories / Core Services (high-value, homepage placement) / Child Services / General Services (link to homepage)
3. PAGE LIST — Homepage, Services, About, Contact, Secondary Category pages, Core Service pages, all Child Service pages
4. INTERNAL LINKING MAP — homepage links; category/core-service → children; child → parent
5. NAVIGATION STRUCTURE — main nav, footer links

OUTPUT FORMAT (exact, so it can be copied into subsequent prompts):
SITE ARCHITECTURE FOR [BUSINESS NAME]
  BASIC INFORMATION — name, industry, city, state, abbrev, zip, phone, email, primary category,
     TARGET KEYWORD: [Primary Category] [City] [State Abbrev]
     SERVICE AREAS / TRUST SIGNALS (suggest 4) / LOCAL ISSUES (suggest 4–5)
  URL STRUCTURE — homepage, main pages (/services /about /contact), secondary category pages, core service pages
  SERVICE HIERARCHY — Secondary Category 1..n (+ child services), Core Service 1..n (+ child services), General Services (→ homepage)
  NAVIGATION STRUCTURE — main nav, footer links
  INTERNAL LINKING MAP — homepage links; each category/core service links to children + back to homepage; child pages link back to parent
  PAGE COUNT SUMMARY — homepage, main pages (3), secondary category, core service, child service, TOTAL

Now analyze my business information and create the complete site architecture.
```

*(Condensed for readability — the live prompt repeats the full output template with `[placeholder]` scaffolding for every field. The structure above is complete.)*

**What it does / output:**
- The **architecture planner / single source of truth** for the whole build. Takes business facts + GBP categories + full service list + service areas and returns one structured `SITE ARCHITECTURE FOR [BUSINESS]` block explicitly designed to be **pasted into every later prompt**.
- Auto-derives: the **TARGET KEYWORD** (`Primary Category + City + State Abbrev`), the homepage **URL slug** (`/[primary-category-slug]-[city-slug]-[state-abbrev]`), a full page list, navigation, a two-way internal-linking map, and a page-count summary.
- **Generates two research artifacts the model is told to *suggest*:** 4 TRUST SIGNALS and 4–5 LOCAL ISSUES for the industry/location. These feed the geographic-relevance/local-expertise content requirements downstream.

**Usage notes:**
- **Inputs required:** business name, industry, city, state, state abbrev, zip, phone, email, primary GBP category, secondary GBP categories, complete service list, service areas.
- **Prerequisite:** assumes GBP categories and services are *already finalized* — it consumes them, it does not discover them. The discovery work is upstream (see cross-refs).
- ⚠️ **This output propagates into Prompts 1–8.** Any error here (wrong category, missing service, bad slug) compounds through every later page. Get this block right before moving on.
- ⚠️ **TRUST SIGNALS and LOCAL ISSUES are AI-suggested** — verify against the real business and real local geography before they get baked into page copy in the content prompts.
- ⚠️ **Service areas are collected but produce no location pages here** — consistent with location pages being Phase 4 (post 30–40% green). Service areas presumably feed geo-relevance copy, not dedicated pages, in this build.

🔄 **Cross-references & overlaps (confirmed):**
- 🔄 **AI Agent Prompt — Local Business Website Builder** (main notes → "INPUTS REQUIRED FROM USER" + "SITE ARCHITECTURE TEMPLATE"). **This is the parent.** Same skeleton (homepage → secondary categories → child services; two-way internal linking). Prompt 0's **"Core Services" = the AI Agent's "Critical Service 1/2 (linked directly from homepage)"** — same concept, renamed. **Divergences:** Prompt 0 strips the AI Agent's strategic intake (no market competitiveness, competitors, population, budget tier, existing-site audit, CMS) and omits the Locations + Supporting Content branches from its output, while **adding a "General Services → homepage" bucket** the AI Agent doesn't name. Net: **Prompt 0 ≈ just the AI Agent's "Site Map" output, generated from minimal inputs.** This course is the modular build path; the AI Agent Prompt is the all-in-one strategist+spec.
- 🔄 **8.1 Local Site Structure Blueprint** (Prompt Catalog). Same architecture concept and identical two-way internal-linking logic. **Divergences:** 8.1's homepage target keyword is `Primary Category + City` (no state); **Prompt 0 adds State Abbrev** and a formal URL-slug convention 8.1 never specifies. 8.1 includes Supporting Content + Location branches; Prompt 0 omits both at the planning stage.
- ⬆️ **Upstream prerequisites (not overlaps):** **3.4 Determine & Organize GBP Categories / P&T #3** and **4.6 Service Entity Research / P&T #4** produce the categories and service list that Prompt 0 *consumes*. Run those first; Prompt 0 does not regenerate them.
- ↔️ **1.4 Website Core 30 Structure Checker / P&T #5** is the *inverse* tool, not a duplicate: 1.4 audits an existing site against the Core 30; Prompt 0 plans a new build from scratch. Complementary.

⚠️ **Title-tag watch:** Prompt 0's TARGET KEYWORD bakes in the **State Abbrev**, but the main-notes title-tag convention is `Primary Category + City | Brand Name` (no state). Flag whether Prompts 2/3 carry the state abbrev into the actual `<title>` or drop it — this is the kind of drift that breaks NAP/title consistency.

**Role in the sequence:**
- **Step 0 — the source of truth.** Produces the master architecture block that Prompt 1 (Skeleton) turns into page shells and that every content/build-out prompt (2–8) reads from. Nothing downstream should contradict this block.

---

# Lovable HTML: NEEDED to Get Ranked (framing lesson)

**Source:** Course lesson is a video; the notes below are corroborated by Dan's external Google/AI-Overview research (May–Apr 2026 sources). ✅ **This closes the crawlability thread flagged in Prompt 8.**

**The core problem (confirmed):** Lovable builds **client-side-rendered (CSR) React + Vite apps.** By default a search bot fetches a near-empty HTML shell (`<div id="root"></div>`) and the real content is painted by JavaScript afterward. Google renders JS slowly and with crawl-budget limits; Bing and AI crawlers (ChatGPT etc. — surfaces this methodology explicitly targets) do it worse or not at all. Result: a beautiful site that indexes terribly. **This is the single dependency the 8-prompt build does not solve on its own.**

**The fix = serve pre-rendered, crawlable HTML to bots.** Two layers:

**A. The two fixes Prompt 8 does NOT cover (the actual gap-closers):**
1. **Server-side pre-rendering / static generation.** Swap CSR for indexable HTML snapshots when a bot visits. Options: Lovable's built-in **"Discoverability"** pre-rendering (launched ~May 13, 2026 — likely the current best native path), or external tools — **LovableHTML** (lovablehtml.com), **Hado SEO** (dynamic rendering: pre-rendered HTML to bots, live app to users), **NextLovable CLI**, or a static deploy via GitHub Pages (~$4/mo).
2. **Host-level deep-route redirect to `index.html` with a 200 status** (Netlify/Vercel config) so deep routes don't return generic 404s to crawlers.

**B. The fixes that OVERLAP Prompt 8 (redundant — Prompt 8 already does these):** dynamic per-route `<title>`/meta, one H1 + H2/H3 hierarchy, sitemap.xml + robots.txt (+ connect to Search Console), JSON-LD schema, WebP + alt text, clean URL slugs.

**The execution prompt (paste into Lovable):**
```
Optimize this entire project for SEO. Ensure a clean semantic HTML structure using exactly one
unique H1 per page and proper H2/H3 hierarchies. Generate dynamic metadata, custom title tags
under 60 characters, and custom descriptions under 160 characters for every route. Clean all URL
paths into SEO-friendly slugs, create a sitemap.xml and robots.txt file, and prepare the code
structure for server-side pre-rendering so that Google can index the full layout text.
```

**Usage notes:**
- ⚠️ **The chat prompt alone is unlikely to produce true SSR.** "Prepare the code structure for server-side pre-rendering" is not the same as actually serving pre-rendered HTML — that happens at the **deployment/hosting/tool layer** (Lovable Discoverability, LovableHTML/Hado, or a prerender-capable host). Treat the prompt as setup; the real fix is the deploy step. **Verify with the bot's-eye view** (Search Console URL Inspection "view crawled page," or curl the URL and check the HTML isn't a blank shell) before trusting rankings.
- ⚠️ **Run this LATE** — after the build and after Prompt 8. The pre-render snapshot must capture finished pages.
- Given Lovable shipped native Discoverability in May 2026, prefer it over the older external-tool workarounds where possible; confirm what your Lovable plan exposes.

🔄 **Cross-references & overlaps:**
- 🔴➡️✅ **Resolves the Prompt 8 SPA-rendering gap.** Prompt 8 does on-page technical SEO assuming HTML content exists; this lesson supplies the rendering layer that makes that content exist for bots.
- 🔄 **Crawlability / Technical Foundation** (AI Agent Prompt + Complete Playbook: "robots.txt allows indexing… clean URL structure… no infinite loops"). This is the **Lovable-specific** mechanism behind that rule — 🆕 on the CSR/pre-render specifics, which the main notes (CMS-agnostic) never address.
- ⚠️ **Heavy redundancy with Prompt 8** on the on-page items — running both repeats sitemap/robots/meta/schema/H1 work. The non-overlapping, essential additions are A1 (pre-render) and A2 (200 redirect).

**Notes:**
- ⚠️ This is the dependency everything else rests on. The whole 8-prompt build's ranking outcome hinges on this one fix being correctly deployed and verified.

---

# Prompt 1 — Skeleton

**Role assigned:** "Senior web developer with 15+ years of experience building SEO-optimized local business websites." *(First non-SEO-strategist persona — this is a front-end build prompt.)*

**The prompt:**

```
You are a senior web developer (15+ yrs, SEO-optimized local business sites). Build the complete
site structure and design system. ARCHITECTURE ONLY — content comes in later prompts.

SITE ARCHITECTURE — PASTE FROM PROMPT 0
[paste the complete Prompt 0 output block here]

DESIGN VARIABLES — COLOR SCHEME (adjust to brand):
  Primary #1E3A5F (dark blue) / Accent #3B82F6 (bright blue) / Background #FFFFFF / Text #1F2937

IMPLEMENTATION INSTRUCTIONS:
1. Branding & Design — use BUSINESS NAME + COLOR SCHEME; clean trustworthy typography;
   "professional but approachable local business — not corporate"
2. Header — top bar ("Serving [CITY], [STATE] & Surrounding Areas" left, [PHONE] click-to-call right);
   main header (logo left, nav center, phone button as primary CTA right); sticky on scroll
3. Navigation — from architecture; simple/clean, NO dropdowns; all items link to defined URLs
4. Footer — phone (click-to-call), address ([CITY], [STATE] [ZIP]), email, all SERVICE AREAS,
   quick links, social placeholders (Facebook, Google), © 2025 [BUSINESS NAME]
5. Mobile — hamburger menu; floating "Call Now" button (bottom-right, always visible);
   click-to-call everywhere; thumb-friendly buttons
6. Page Creation — create ALL pages from architecture (homepage, Services/About/Contact,
   all secondary category, all core service, all child service, all general service pages)
7. Placeholder Content — each page shows ONLY: page title ("[Service] [City] [State Abbrev]"),
   "Content coming soon", header + footer. Do NOT write real content.
8. Services Page — /services lists links to ALL service pages organized by SERVICE HIERARCHY (verification)
9. Scroll Behavior (CRITICAL) — implement a ScrollToTop component resetting scroll to (0,0) on every
   route change; users must always land at the top of each page
10. Technical — mobile-first responsive; fast; clean semantic HTML5; all nav links working;
    consistent header/footer; EVERY architecture page must be a real route
11. Verification — page count matches PAGE COUNT SUMMARY; all routes accessible; nav works; ScrollToTop works

Generate the complete site structure, navigation working, placeholder text only.
```

**What it does / output:**
- The **front-end scaffolding prompt**, run in **Lovable**. Consumes the Prompt 0 architecture block and builds the entire empty site shell in one shot: a **design system** (color tokens + typography direction), a **header** (sticky; "Serving [City], [State] & Surrounding Areas" top bar + phone CTA), a **footer** (full NAP + service areas + quick links + social placeholders), **mobile UX** (hamburger, always-visible floating "Call Now," click-to-call), and **every page from the architecture created as a real route** carrying only a title + "Content coming soon."
- `/services` doubles as a **verification sitemap** — every service link, organized by the Prompt 0 hierarchy.
- Mandates a **ScrollToTop component** (reset to `(0,0)` on route change), flagged *Critical*.
- Ends with a **self-verification checklist** (page count vs. summary, routes accessible, nav + ScrollToTop working).

**Usage notes:**
- **Inputs:** the full Prompt 0 output block + a color scheme (defaults provided = the dark-blue palette seen in the Gary demo; adjust to brand).
- **Build environment confirmed = Lovable / React SPA.** The mandated `ScrollToTop`-on-route-change is a React-Router tell — this is client-side routing, which is exactly the setup the "Lovable HTML: NEEDED to Get Ranked" lesson exists to make crawlable.
- **Deliberately content-free** — placeholder text only; all real copy arrives in Prompts 2–8. This locks in the **scaffold-everything-first, fill-later** workflow.
- ⚠️ **Hardcoded `© 2025`** — it's 2026; update the footer year or the prompt.
- ⚠️ **Thin-content-at-scale risk.** This builds the *entire* Core 30 (every category + service page) up front as live routes showing "Content coming soon." The main notes explicitly caution against building too fast and against thin content. **Fill content before exposing these routes to crawlers / before launch** — don't let dozens of placeholder pages get indexed.

**Cross-references & overlaps:**
- 🆕 **The scaffolding mechanics are net-new to your library.** Routes, design tokens, sticky header, floating call button, hamburger nav, ScrollToTop, semantic-HTML build — none of this exists in the main notes, which are SEO/content/strategy, not front-end build. This is the course's genuine new contribution.
- 🔄 **Technical Foundation** (AI Agent Prompt → "TECHNICAL FOUNDATION REQUIREMENTS" + *Complete Playbook* → "Technical Foundation"). The header/footer NAP, every-phone-a-`tel:`-link, click-to-call, mobile-first responsive, clean semantic HTML5, and working internal links all **operationalize the documented technical-foundation rules at the skeleton stage** rather than as a final audit.
- ⬅️ **Consumes Prompt 0 wholesale** (page list, navigation, internal-linking map, NAP, service areas). Confirms the source-of-truth handoff — Prompt 1 transforms the plan into structure, adds nothing strategic.
- ➡️ **Forward link to the Lovable HTML lesson + Prompt 8 (Technical SEO):** the SPA routing this prompt sets up is precisely what those lessons must make crawlable/indexable.

⚠️ **Title-tag watch (update):** Prompt 1's placeholder page-title format is `"[Service Name] [City] [State Abbrev]"` — **the State Abbrev persists into the skeleton's titles**, reinforcing the divergence from the `Primary Category + City | Brand Name` convention. Still placeholder text, so the *real* `<title>` is set in Prompts 2/3 — keep watching, but the trend is toward keeping the state abbrev.

**Role in the sequence:**
- **Step 1 — the empty, fully-routed, fully-branded shell.** Turns the Prompt 0 plan into a navigable site with every page existing but empty. Prompts 2–7 each pour content into one page type; Prompt 8 does the technical pass.

---

# Prompt 2 — GBP Landing Page Content

**Role assigned:** "Expert conversion copywriter who specializes in local service businesses." Core thesis stated up front: the homepage exists for ONE purpose — get the searcher to call or submit a form.

**The prompt:**

```
You are an expert conversion copywriter (local service businesses). The homepage exists for ONE
purpose: get the searcher to call or submit a form. Speak DIRECTLY to the searcher's problem;
position the business as the obvious choice through specific proof, not generic claims.

SITE ARCHITECTURE — PASTE FROM PROMPT 0
[paste Prompt 0 block]

BUSINESS DIFFERENTIATORS — answer with SPECIFIC, PROVABLE claims (10 questions):
  1 #5-star reviews / 2 avg response time / 3 free estimates? / 4 trip fee? / 5 24/7 or after-hours?
  6 years serving area / 7 guarantees / 8 licenses+certs / 9 locally/family owned? / 10 what makes you different

GOAL COMPLETION FRAMEWORK — every section answers ONE question in the searcher's mind:
  Hero: "Can you solve my problem right now?"  | Why Choose Us: "Why YOU over everyone else?"
  Reviews: "Do other people trust you?"        | Services: "Do you handle what I need?"
  FAQ: "What concerns before calling?"
  (The searcher has a problem and is scanning for PROOF. They don't care about your company history.)

CONTENT TO GENERATE:
  SECTION 1 HERO — H1 (include [PRIMARY CATEGORY]+[CITY]+[STATE ABBREV], outcome-focused, 60–70 chars;
     3 formula options) + Subheadline (proof + promise + CTA, 15–20 words)
  SECTION 2 WHY CHOOSE US — 4 differentiators (provable headline + 1–2 sentences; use numbers;
     GOOD vs BAD examples; "Licensed & Insured" = table stakes, belongs in trust bar not here)
  SECTION 3 SECONDARY CATEGORY DESCRIPTIONS — per category: 2–3 sentences, problem-focused, mention [CITY]
  SECTION 4 CORE SERVICE HIGHLIGHTS — per core service: 3–4 sentences positioning as specialty
  SECTION 5 ABOUT/CREDENTIALS — NOT history; 3–4 sentence credibility statement
  SECTION 6 FAQ — 5–6 Qs phrased as the customer asks (cost/timing/trust/process); answer-first
  SECTION 7 FINAL CTA — headline (5–8 words) + subtext (1 sentence) + phone prominent

OUTPUT FORMAT — organize under clear headings so it can be copied directly into Prompt 3.

WHAT NOT TO WRITE — no "Welcome to [Business]"; no founding story in hero; no "We pride ourselves";
  no generic differentiators (quality/experience/satisfaction); no jargon; no long paragraphs;
  no "Contact us today for all your [industry] needs."
```

**What it does / output:**
- The **homepage copy generator**. Takes the Prompt 0 block + a **10-question differentiator intake** (review count, response time, trip fee, guarantees, licenses, etc.) and produces seven labeled content blocks — Hero (H1 + subheadline), 4 Why-Choose-Us differentiators, secondary-category descriptions, core-service highlights, an about/credibility paragraph, 5–6 FAQs, and a final CTA — structured to **paste straight into Prompt 3**.
- Built entirely around the **Goal Completion Framework**: each section answers exactly one question the searcher is scanning for. Heavy use of GOOD vs. BAD examples to force specificity over fluff.

**Usage notes:**
- **Inputs:** Prompt 0 block + the 10 provable differentiator answers. Quality of output is capped by how specific those 10 answers are — vague answers produce the generic copy the prompt is trying to avoid.
- **Generates H1, not the `<title>` tag.** Prompt 2 writes the visible H1 only; the meta `<title>` still hasn't been authored anywhere (expect it in Prompt 3 build-out or Prompt 8).
- ⚠️ **MISSING the canonical "Words to Avoid" list.** This is the actionable one. Prompt 2 has its own short "WHAT NOT TO WRITE" (no "Welcome to," no fluff) but does **not** include the long banned-word list (embark, delve, crucial, ensure, comprehensive, etc.) that your **2.1 / AI Agent Prompt carry — and that's on your own standing content-preference list.** Output from Prompt 2 will not be scrubbed for those AI-tell words unless you append the list yourself. **Recommend: paste your avoid-words list into the WHAT NOT TO WRITE section before running.**
- ⚠️ **Trust-signal reconciliation.** Prompt 0 had the model *suggest* 4 trust signals (AI guesses). Prompt 2 now collects *real, provable* differentiators from you. Make sure the Prompt 2 reality replaces the Prompt 0 guesses — don't let invented Prompt 0 trust signals survive into the page.

**Cross-references & overlaps:**
- 🔄 **2.4 Goal Completion Content Rewrite / P&T #2** — same conceptual root. 2.4 rewrites *one* fluffy block into <50 punchy words (service+city first, CTA second). Prompt 2 **scales that principle across the entire homepage**, section by section. Not a duplicate — the section-level expansion of the goal-completion idea.
- 🔄 **2.1 Local SEO Content Writer / P&T #1** — alternative homepage-content approach, different philosophy. 2.1 is length-driven (~1,500 words, keyword density, mentions all categories/services in flowing copy, carries the banned-words list). Prompt 2 is **conversion-driven** (structured sections, differentiator proof, GOOD/BAD examples, no word-count target). Two different ways to fill the same page — Prompt 2 optimizes for the call, 2.1 optimizes for topical coverage.
- 🔄 **Homepage (GBP Landing Page) spec — AI Agent Prompt + Complete Playbook.** Prompt 2 is the **content layer** of that spec. Direct matches: H1 = category+city, "cut Welcome to / company history," "speak TO the searcher not ABOUT the business," per-secondary-category copy, social proof high. **Not covered by Prompt 2** (handled by Prompt 1 skeleton / Prompt 3 build-out / Prompt 8): NAP placement, LocalBusiness schema, GBP map embed, reviews-score embed, the under-50-words-above-fold limit, and 5th-grade reading level. Clean division of labor.
- 🔄 **2.5 Determine Searcher Intent** — the "Goal Completion Strategy" column there (what appears above the fold to satisfy the user) is the same framework Prompt 2 builds the page around. Running 2.5 first on the target keyword would sharpen which goal-completion elements Prompt 2 should emphasize.

⚠️ **Title-tag watch (update):** Prompt 2's H1 requirement says include `[PRIMARY CATEGORY] + [CITY] + [STATE ABBREV]`, but its own formula options and worked example ("Gary's Most Trusted Plumber | 500+ Five-Star Reviews") **omit the state** — the prompt is internally inconsistent on the abbrev. And this is the H1, not the `<title>`. So: state abbrev is *required in the H1 instruction* but *dropped in the examples*, and the real `<title>` still isn't set. **Still unresolved — watch Prompt 3.**

**Role in the sequence:**
- **Step 2 — homepage content only.** Produces labeled copy blocks. Hands directly to **Prompt 3 (GBP Landing Page Build Out)**, which places this copy into the skeleton's homepage route with the structural/technical elements.

---

# Prompt 3 — GBP Landing Page Build Out

**Role assigned:** "Senior web developer implementing a homepage... content already written; implement with structure, design, and technical SEO that MAXIMIZE CONVERSIONS."

**Notable preamble:** The lesson shows Caleb *revising* this prompt after reverse-engineering **Zehl & Associates' homepage** (a personal-injury law firm) — "lead with proof not promises." The mandatory section order below is derived from that teardown (credibility → form → testimonials → education last). Worth noting the example flips from the plumber to a law firm purely to source the conversion formula.

**The prompt:**

```
You are a senior web developer implementing a homepage for a local service business. Content is
already written — implement it with structure, design, and technical SEO that MAXIMIZE CONVERSIONS.

SITE ARCHITECTURE — PASTE FROM PROMPT 0      [paste]
PRE-WRITTEN CONTENT — PASTE FROM PROMPT 2     [paste]

GOAL COMPLETION HIERARCHY — page exists to get a call/form. Social proof + credibility FIRST,
educational content LAST. Every section answers "Why choose THIS company?"

SECTION ORDER (MANDATORY):
 1 HERO — generated [INDUSTRY] bg image + dark overlay; H1 EXACTLY; subheadline EXACTLY;
    primary CTA "Call Now [PHONE]" (click-to-call); secondary CTA "Get Free Estimate";
    trust strip: Licensed & Insured | 24/7 Emergency | Same-Day Service | [additional]
 2 WHY CHOOSE US — "Why [CITY] Homeowners Call Us First"; 4 icon boxes (specific differentiators)
 3 GOOGLE REVIEWS EMBED — "See What Our Customers Say"; placeholder div + <!-- PASTE EMBED --> (high on page)
 4 LEAD CAPTURE FORM — "Get Your Free Estimate"; Name/Phone/Email/Service(dropdown from architecture)/Message;
    prominent + contrasting bg; "No obligation. Response within 1 hour during business hours."
 5 SECONDARY CATEGORY CARDS — pre-written H2; card per category → links to category page
 6 CORE SERVICE HIGHLIGHTS — pre-written H2; more prominent styling than categories → links to service pages
 7 SERVICE AREA SECTION — "Proudly Serving [CITY] and [STATE/REGION]"; compact, informational
 8 ABOUT/CREDENTIALS — "Your Local [INDUSTRY] Experts"; pre-written about; team/owner photo space
 9 FAQ — "Common Questions"; accordion; + LocalBusiness FAQ schema
 10 LOCATIONS WE SERVE — compact, just above footer; link to /locations/ hub; NOT prominent
 11 FINAL CTA — contrasting bg; "Ready to Get Started?"; phone prominent; Call Now + Schedule Online; hours

TECHNICAL:
  Title: "[TARGET KEYWORD] | 24/7 Emergency Service | [BUSINESS NAME]"
  Meta desc: "[CITY]'s most trusted [PRIMARY CATEGORY]. [Key differentiator]. Call [PHONE] for same-day service."
  H1: from pre-written (EXACTLY)
  Schema: LocalBusiness (full NAP) + Service (core services) + FAQ
  Mobile: click-to-call; mobile-sized form; sticky mobile CTA bar at bottom
  Performance: lazy-load below-fold images; optimize hero image

WHAT NOT TO DO: no About/history high; no "Quality Service Since 2005"; don't bury reviews/testimonials;
  service-area section not a major visual; no stock-photo carousels (one hero image); no extra sections.
```

**What it does / output:**
- The **homepage implementation prompt**, run in Lovable. Merges the Prompt 2 copy (used *exactly*) into the skeleton's homepage route as a fully-built, conversion-ordered page: generated hero image + overlay, dual CTAs, trust strip, 4 differentiator boxes, reviews-embed placeholder, prominent lead form, category + core-service cards, service-area + locations sections, accordion FAQ, final CTA.
- **Authors the meta layer for the first time:** `<title>`, meta description, and confirms the H1 — plus LocalBusiness + Service + FAQ schema, a sticky mobile CTA bar, and lazy-loading.

**Usage notes:**
- **Inputs:** Prompt 0 architecture + Prompt 2 content (both pasted). Content is placed verbatim — Prompt 3 does layout/structure/technical, not rewriting.
- ⚠️ **Hardcoded "24/7 Emergency Service" / "Same-Day Service" — generalization trap.** The title template, the hero trust strip, and the meta description all bake in emergency-trade language. **This fits plumbing/HVAC/restoration; it is wrong for non-emergency businesses.** For your own sites — **Crowley's countertops and Portland Gutter Cleaner are not 24/7 emergency / same-day services** — you must replace these segments or the title and trust signals will be false. Edit before running on anything that isn't an emergency trade.
- ⚠️ **Title length.** `Plumber Gary IN | 24/7 Emergency Service | Gary Plumbing Company` ≈ 62 chars — over the **under-60-character** cap in your main notes' title conventions. The three-part structure tends to overflow; trim the middle segment or the brand.
- ⚠️ **Locations hub mismatch.** Section 10 links to a `/locations/` hub and Section 7 references location links, but Prompt 0 and the Prompt 1 skeleton **built no location pages** (deferred to Phase 4). The homepage points at a hub the architecture didn't create. Either treat as "if it exists" or hold these links until Phase 4.
- ⚠️ **Schema starts here, not in Prompt 8.** Per-page LocalBusiness/Service/FAQ schema is injected at build-out. Watch for **duplication or conflict** when Prompt 8 (Technical SEO Implementation) runs its pass — confirm Prompt 8 audits/dedupes rather than re-adds.
- New build mechanics: AI-generated hero image, sticky mobile CTA bar, accordion FAQ, lead-form-as-section.

**Cross-references & overlaps:**
- 🔄 **GBP Landing Page Quick Hits** (GBP Optimization Materials) — **Prompt 3 satisfies all 9 checklist items**: above-fold goal completion (§1), social proof high (§2–3), NAP match (footer + schema), LocalBusiness schema, title tag w/ category+city, H1 w/ city, speak-TO-the-searcher, review embed near top (§3), working click-to-call. Cleanest 1:1 map in the course so far.
- 🔄 **Homepage (GBP Landing Page) spec — AI Agent Prompt + Complete Playbook.** Prompt 3 is the structural/technical execution of that spec. **One real omission:** the AI Agent spec requires a **GBP map embed** (separate from the reviews embed); Prompt 3 includes the reviews embed (§3) but **no map embed**. Add it manually if you want spec parity.
- 🔄 **Goal Completion (2.4 / 2.5)** — here the principle governs **section ORDER** (proof first, education last), not just copy. The Zehl teardown is "Determine Searcher Intent" (2.5) done by hand on a single winning page.
- 🆕 **Net-new:** the Zehl-derived 11-section conversion order, generated hero imagery, sticky mobile CTA bar, lead-capture-form-as-section. No prior asset specifies homepage *layout order*.
- ⬅️ **Consumes Prompt 2 "EXACTLY" + Prompt 0.** Confirms the content→build-out handoff is literal (no rewriting at build time).

✅ **Title-tag drift — RESOLVED.** The real `<title>` = `[TARGET KEYWORD] | 24/7 Emergency Service | [BUSINESS NAME]`, and since TARGET KEYWORD = `Primary Category + City + State Abbrev`, **the state abbrev IS retained** (e.g., "Plumber Gary IN | …"). This **diverges from your main-notes convention** (`Primary Category + City | Brand`, under 60 chars) on three counts: (1) adds the state abbrev, (2) inserts a hardcoded middle qualifier, (3) runs long. Decide which convention you standardize on for your own builds.

**Role in the sequence:**
- **Step 3 — the first fully-built page.** Homepage is now live with copy, layout, schema, meta, and mobile conversion elements. Prompts 4–7 replicate the build-out pattern for the remaining page types; Prompt 8 does the site-wide technical pass.

---

# Prompt 4 — Secondary Category Page Build Out

**Role assigned:** "Senior web developer and local SEO expert." *(Combined persona — this prompt writes content AND builds, unlike the homepage's split.)*

**The prompt:**

```
You are a senior web developer and local SEO expert. Create complete secondary category pages with
content, structure, and internal linking. Category pages link DOWN to child services and UP to homepage.

SITE ARCHITECTURE — PASTE FROM PROMPT 0      [paste]   ← NOTE: no content paste; content generated here

Create a page for EACH Secondary Category in the SERVICE HIERARCHY. For each:
1 SEO META — Title "[Category] [City] [State Abbrev] | Fast, Reliable Service";
   meta desc 150–160 chars targeting "[Category] [City]"; H1 "[Category] in [City] [State Abbrev] — [Benefit]"
2 HERO — generated category-relevant background image (NOT solid color) + dark overlay; H1;
   subheadline 2–3 sentences (problem + mention 24/7 + same-day + phone); Call Now + Schedule Service; trust signals
3 CONTENT (1,000–1,200 words):
   Opening (3–4 sentences: user frustration, what they tried, right place, urgency)
   H2 "What [Category] Problems Do You Have?" (150–200w; problems, warning signs, why DIY fails, ref LOCAL ISSUES)
   H2 "Our [Category] Services" (200–300w; mention EVERY child service by exact name → become links; flowing prose, no bullets)
   H2 "[Category] for [City] Homes/Businesses" (150–200w; ref SERVICE AREAS; local expertise)
   H2 "Why Choose Us for [Category]" (100–150w; ref TRUST SIGNALS; fast response, same-day, upfront pricing)
   Final CTA (urgency + phone); Homepage link (use HOMEPAGE ANCHOR TEXT OPTIONS from architecture)
4 INTERNAL LINKING (critical) — every child service name hyperlinked to its URL; homepage link; clean URLs, no #
5 SERVICES GRID — after content, grid of all child services (name, 1-sentence desc, "Learn More →" link)
6 SCHEMA — Service JSON-LD (@type Service, serviceType [Category], provider→LocalBusiness, areaServed [City],[State])
7 SCROLL — links load at TOP, no anchor links
8 SECTION ORDER — hero → opening → problems → services(links) → for-city → why-us → grid → final CTA → footer

CONTENT GUIDELINES: Google (category+city in H1/first para; each child service by exact name; local refs);
   AI systems (local expert, conversational, helpful); language 5th grade, short sentences, not salesy.
Words to AVOID: embark, look no further, top-notch, comprehensive, delve, crucial, vital, seamless,
   cutting-edge, leverage, robust, game-changer, nestled, we understand, testament
```

**What it does / output:**
- Builds **every secondary category page** in one pass — **content generation AND implementation combined** (no separate content prompt). Each page: generated hero image, ~1,000–1,200 words across a fixed 4-H2 structure, a child-services grid, Service schema, and the DOWN-to-children / UP-to-homepage linking.
- **Pulls heavily from the Prompt 0 architecture block** for its content: LOCAL ISSUES, SERVICE AREAS, TRUST SIGNALS, and HOMEPAGE ANCHOR TEXT OPTIONS are all referenced as content inputs.

**Usage notes:**
- **Input is the Prompt 0 block ONLY** — no Prompt 2-style content paste. ⭐ **This confirms the workflow asymmetry: the homepage is the only page type that gets a dedicated content prompt (2) + build prompt (3). Every other page type generates content inline during build-out.**
- ⚠️ **Banned-words list is present but DIFFERENT and shorter.** Prompt 4 carries a **15-word** avoid list (embark, look no further, top-notch, comprehensive, delve, crucial, vital, seamless, cutting-edge, leverage, robust, game-changer, nestled, we understand, testament). This **partially overlaps** your canonical/preference list but adds words it doesn't have (seamless, cutting-edge, leverage, robust, game-changer, nestled) and **omits many it does** (ensure, optimal, in conclusion, furthermore, moreover, etc.). Combined with **Prompt 2 having no list at all**, the course is internally inconsistent on banned words. **Standardize: paste your full avoid-words list into every content-generating prompt.**
- ⚠️ **Trust-signal source mismatch (coherence risk).** The homepage (Prompt 3) shows your *real, provable* differentiators from the Prompt 2 intake. Category pages (Prompt 4) pull TRUST SIGNALS from the **Prompt 0 architecture block** — which may still hold Prompt 0's *AI-guessed* trust signals if you never reconciled them. Result: homepage and category pages could advertise different trust claims. Fix the Prompt 0 block to hold the real signals before running Prompt 4.
- ⚠️ **Input-chain gap: "HOMEPAGE ANCHOR TEXT OPTIONS."** Prompt 4 expects this from the architecture, but Prompt 0's output template doesn't clearly generate it. Add anchor-text options to your Prompt 0 block, or Prompt 4 will improvise them.
- ⚠️ **Qualifier drift between page types.** Title qualifier is **"Fast, Reliable Service"** here vs. **"24/7 Emergency Service"** on the homepage (Prompt 3). And the hero subheadline still hardcodes "24/7 and same-day." Same emergency-trade trap — **wrong for Crowley's / gutter cleaning; edit per business.**
- ✅ **5th-grade reading level** appears here (it was missing from Prompt 2's content rules).
- State abbrev retained in both title and H1 (consistent with the Prompt 3 resolution).

**Cross-references & overlaps:**
- 🔄 **Secondary Category Pages spec — AI Agent Prompt + Complete Playbook.** Clean implementation: H1 category+city ✓, title Category+City+qualifier ✓, full category scope ✓, links DOWN to every service ✓, link UP to homepage ✓, category-specific local refs ✓, CTA ✓. Prompt 4 adds the fixed 4-H2 content skeleton, word count, services grid, and schema the spec leaves unspecified.
- 🔄 **The Internal Linking Mirror / Internal Linking Rules (Module 3 + AI Agent).** "Category pages link to homepage + all service pages under that category" — implemented exactly (every child service name becomes a link; homepage link; no `#` anchors, consistent with the Prompt 1 ScrollToTop rule).
- 🔄 **2.1 Local SEO Content Writer / P&T #1.** Prompt 4 ≈ 2.1's *secondary-category adaptation* ("remove the secondary categories section, only list services under this one category") fused with build-out. Same dual-audience (Google + AI), local-reference, page-type-scaled-length philosophy.
- 🔄 **CONTENT GENERATION RULES (AI Agent Prompt).** Dual-audience writing, 5th-grade level, words-to-avoid all mirror — but with the shorter, divergent avoid list noted above.
- ⚠️➡️ **Tension with the AI Agent "Service Pages" tone rule (matters for Prompt 5/6).** That spec says **vary tone by service type** — emergency → urgency; **high-ticket → options, decision factors, investment framing**; routine → concise. This course **hardcodes emergency/same-day framing across page types.** For **high-ticket, non-emergency work like Crowley's countertops, the canonical spec calls for investment framing, not "24/7 emergency."** Flag this hard when Prompts 5–6 (service pages) arrive.
- 🆕 **Net-new:** combined content+build single-prompt-per-page-type pattern, generated category hero images, the services-grid section.

**Role in the sequence:**
- **Step 4 — all secondary category pages, content + build in one shot.** Establishes the repeatable template (hero image → fixed H2 structure → grid → schema → linking) that Prompts 5–7 reuse for the other page types.

---

# Prompt 5 — Core Service Page Build Out

**Role assigned:** "Senior web developer and local SEO expert." Core service pages = "high-value service hubs that link DOWN to related child services and UP to the homepage."

**This is a crisis/urgency-tuned twin of Prompt 4.** Same combined content+build model, same Prompt-0-only input, same 1,000–1,200 words, same hero/grid/schema/scroll/linking machinery and verification checklist. Rather than repeat it, here are the deliberate **deltas vs. Prompt 4**:

| Element | Prompt 4 (Category) | Prompt 5 (Core Service) |
|---|---|---|
| Title qualifier | `\| Fast, Reliable Service` | `\| Same-Day Service Available` |
| H1 phrase | `— [Benefit Phrase]` | `— [Urgency/Benefit Phrase]` |
| Meta desc | targets "[Category] [City]" | "emphasizing fast resolution" |
| Hero subheadline | "user's problem... 24/7 + same-day" | "user's **crisis/urgent situation**, emphasizing speed" |
| Opening para | frustration / what they tried | "**urgent situation... disruption to their life... isn't a wait-and-see problem**" |
| H2 structure | Problems / Our Services / For City / Why Us (**4**) | Signs You Need / Our **Options** / For City / **What to Expect** / Why Us (**5**) |
| Decision content | — | "repair vs replacement," "when someone would choose each option," diagnosis→timeline |
| Internal linking | DOWN to children + UP to homepage | + **LATERAL link to related Secondary Category** (if in architecture) |
| Avoid-words list | 15 words | **16 words** (adds "state-of-the-art") |
| Section order | 9 | 10 (extra "What to Expect") |

**What it does / output:**
- Builds **every Core Service page** — the high-value individual services promoted to homepage-level prominence (vs. grouped under a category). Each is a hub with its own child services beneath, now also **cross-linking laterally to a related secondary category**. The content adds genuine decision-support structure ("Signs You Need," repair-vs-replacement, "Our Options," "What to Expect").

**Usage notes:**
- **Resolves the Core-vs-Service question fully:** both categories (Prompt 4) and core services (Prompt 5) are *hubs with children*; the difference is core services are individual high-value services elevated to homepage links, whereas categories group services. Prompt 6 builds the leaf/child service pages beneath both.
- ⚠️ **Qualifier drift is now three-way:** "24/7 Emergency Service" (homepage) → "Fast, Reliable Service" (category) → "Same-Day Service Available" (core service). All hardcoded. Edit per business.
- ⚠️ **Avoid-words list grew to 16** (added "state-of-the-art") and still doesn't match Prompt 4's 15, Prompt 2's zero, or your canonical list. The inconsistency is now confirmed across four prompts. **Paste your full list every time.**

🔴 **The tone-by-service-type tension lands HERE — this is the most important finding for Crowley's.**
- The AI Agent spec's Service Pages rule says **high-ticket services get "options, decision factors, investment framing,"** not urgency. Prompt 5 instead hardcodes **crisis framing** for *all* core services: "crisis/urgent situation," "disruption to their life," "this isn't a wait-and-see problem," "Same-Day Service Available."
- **For Crowley's countertops — a high-ticket, planned, high-consideration purchase — this framing is backwards.** Nobody is in "crisis" over a countertop; "same-day" is false and "wait-and-see" reframing misreads the buyer.
- **The fix is surgical, not wholesale:** Prompt 5 already contains the *right* bones for high-ticket — "Our Options," "when someone would choose each option," "What to Expect," repair-vs-replacement. **Keep that decision structure; strip the crisis/urgency/same-day language and swap in investment framing** (cost ranges, material/edge/sink options, timeline expectations, the ~$5k small-kitchen / ~$8k larger-kitchen budget guidance). That single edit makes Prompt 5 fit a considered purchase.

**Cross-references & overlaps:**
- 🔄 **Service Pages spec — AI Agent Prompt + Complete Playbook** (single-service focus, H1 service+city, title service+city+qualifier, links UP to parent + homepage). Implemented — with the urgency-tone override flagged above.
- 🔄 **Module 3, Lesson 3 — Single-Prompt Content Creation** + **2.1 Local SEO Content Writer / P&T #1.** Same single-prompt-per-page content engine; Prompt 5 fixes the structure and fuses build-out.
- 🔄 **Internal Linking Rules** — adds the lateral category cross-link, slightly richer than the strict DOWN/UP mirror.
- 🆕 Decision-support content blocks ("Signs You Need," "What to Expect," repair-vs-replacement) as a fixed template; lateral hub cross-linking.

**Role in the sequence:**
- **Step 5 — all Core Service hub pages.** Same template family as Prompt 4, tuned for urgency. Prompt 6 then builds the child/leaf service pages these hubs link down to.

---

# Prompt 6 — Service Page Build Out

**Role assigned:** "Senior web developer and local SEO expert." Two parts: **Part 1** builds the `/services` hub; **Part 2** builds **every child/leaf service page**. Child pages link UP to their parent.

**This is the Core 30 volume engine.** Part 2 creates an individual page for *every* child service under every Secondary Category, every Core Service, AND every General Service — the bulk of the page count. It's a third near-twin of the Prompt 4/5 build-out template, lighter per page, plus the hub.

**Part 1 — `/services` hub:**
- Title `"[INDUSTRY] Services [City] [State Abbrev] | Complete Service List"`; H1 `"[INDUSTRY] Services in [City] [State Abbrev] — Full-Service [PRIMARY CATEGORY] for Every Job"`.
- **Hero exception:** solid color OR subtle image is *acceptable here* — the **only** page type where a generated hero image isn't mandatory.
- One linked section per grouping (each Secondary Category / Core Service H2 links to its hub page; General Services grouped under "General [INDUSTRY] Services"), each with a card grid of child services. This is the real navigation hub that replaces the Prompt 1 skeleton's placeholder `/services` verification list.

**Part 2 — child service pages (deltas vs. Prompt 5):**

| Element | Core Service (P5) | Child Service (P6) |
|---|---|---|
| Word count | 1,000–1,200 | **600–800** (lighter leaf pages) |
| Title qualifier | `\| Same-Day Service Available` | `\| Fast, Professional Service` |
| H2 structure | Signs / Options / For City / What to Expect / Why Us (5) | When You Need / Our Process / **Cost in [City]** / Why Us (4) |
| Cost section | — | **"[Service] Cost in [City]" — factors + upfront quotes, "Do NOT list specific prices"** |
| Linking | DOWN to children + lateral category | **UP to parent only** (category / core service / homepage for general) |
| Avoid-words | 16 | **back to 15** (drops "state-of-the-art") |

**What it does / output:**
- Builds the `/services` hub + every leaf service page. Leaf pages use the familiar hero/schema/scroll/linking machinery at ~600–800 words with a 4-H2 body, and each links UP to its correct parent per the Prompt 0 INTERNAL LINKING MAP (Secondary Category child → category page; Core Service child → core service page; General Service → homepage).

**Usage notes:**
- ⚠️ **"Do NOT list specific prices" conflicts with your standing copy preference.** The Cost-in-[City] section explicitly forbids concrete prices. **Your documented Crowley's site preference is the opposite** — include simple budget expectations (~$5k small kitchen, ~$8k larger kitchen). If you run this for Crowley's, override this instruction to add the budget guidance; the course default would strip it.
- ⚠️ **Title qualifier drift is now FIVE-way:** "24/7 Emergency Service" (home) / "Complete Service List" (services hub) / "Fast, Reliable Service" (category) / "Same-Day Service Available" (core service) / "Fast, Professional Service" (child service). All hardcoded.
- ⚠️ **Avoid-words list literally fluctuates:** P2 = 0, P4 = 15, P5 = 16, P6 = 15. Final confirmation that the course's banned-words handling is inconsistent. **Paste your full list into every content prompt.**
- ⚠️ **Supporting Content layer is omitted.** Your 8.1 Blueprint's Core 30 includes **2 supporting-content pieces per high-priority service** (PAA pages, educational deep-dives). Prompt 6 builds service pages but **no supporting-content branch**. If you want the full blueprint, that layer is separate work this course doesn't cover.
- Leaf hero still requires a generated image (only the `/services` hub is exempt).

**Cross-references & overlaps:**
- 🔄 **Service Pages spec — AI Agent Prompt + Complete Playbook** (single-service focus, H1/title service+city+qualifier, UP to parent + homepage). Implemented. The leaf "Cost in [City]" section is a course-specific addition; the spec's tone-by-type rule still partly overridden by the same-day/urgency defaults (milder here than Prompt 5).
- 🔄 **Module 3 — Core 30 System** + **1.4 Website Core 30 Structure Checker / P&T #5.** ⭐ **This is the build half of the Core 30.** Module 3 is the framework; 1.4 audits which pages exist; **Prompt 6 generates the full set.** The child service pages *are* the Core 30 volume.
- 🔄 **8.1 Local Site Structure Blueprint → "GBP Service Pages" layer.** Prompt 6 builds that layer — but **not** the blueprint's "Supporting Content Pages" branch (noted above).
- 🔄 **Internal Linking Mirror / Rules.** UP-to-parent + General→homepage implemented exactly per the Prompt 0 map.
- 🆕 The `/services` hub build, the "Cost in [City]" no-prices section, the lighter 600–800-word leaf template.

**Role in the sequence:**
- **Step 6 — the Core 30 page volume + the `/services` hub.** After this, every content page exists. Remaining: `/about` + `/contact` (Prompt 7) and the site-wide technical pass (Prompt 8).

---

# Prompt 7 — About and Contact Page Build Out

**Role assigned:** "Senior web developer and local SEO expert." Two parts: **About** (E-E-A-T credibility) + **Contact** (clear ways to reach the business).

**What it does / output:**
- **Part 1 — `/about`:** a placeholder-driven E-E-A-T page (Our Story, Meet the Owner/Team bio box, optional owner video, Service Area, Credentials & Trust, GBP embed, social links).
- **Part 2 — `/contact`:** two-column layout (contact info | form), service-area list, Google Maps embed, trust reinforcement, ContactPage/LocalBusiness schema, form-handler placeholder.
- Both heroes are "clean (solid or subtle image acceptable)" — so the **generated-image-required rule applies only to homepage + category + core + child service pages**, not to `/services`, `/about`, or `/contact`.

**Usage notes:**
- ⭐ **The About page is deliberately placeholder-driven, and that's correct.** Unlike the service pages (AI-generated content), the About page is mostly HTML-comment placeholders telling *you* to add the real story, real owner bio, real headshot ("not stock"), real license numbers, real video. **This is the right design** — E-E-A-T is unfakeable real-person evidence; AI can't generate a genuine owner story or verifiable credentials. Budget ~2–4 hours of human fill (matches 8.3's one-time-investment note). Don't let it ship with placeholders live.
- ✅ **Schema-dedup awareness is present.** The About-page schema instruction reads "LocalBusiness schema (**if not already on homepage**) or Organization schema." So the course *is* conscious of not double-adding LocalBusiness schema — it conditions it. Good sign for the Prompt 8 question, though the final audit still needs confirming.
- 🗺️ **The Google Maps embed lives on `/contact`** (Part 2, Map Section). This partially answers the earlier "map embed missing" flag: the site *has* a map, just on Contact rather than the homepage. ⚠️ The AI Agent spec wanted the GBP map embed on the **homepage** (GBP landing page) for a local business — that homepage gap still stands; the Contact map doesn't replace it.
- ⚠️ Minor emergency-trap residue: Contact meta description and trust strip still say "same-day service" / "Available 24/7 for emergencies (or appropriate hours)." Edit for non-emergency businesses (Crowley's, gutter cleaning).
- **Form needs a backend.** The contact form is front-end only with a placeholder for Formspree / Netlify Forms / your CRM. Lovable won't wire submissions for you — connect a handler or leads vanish.

**Cross-references & overlaps:**
- 🔄 **8.3 E-E-A-T About Page Checklist (Prompt Catalog) — near-complete implementation. The cleanest catalog-asset → build-template mapping in the course.** All 6 checklist items present:
  1. Method to get in contact → hero phone + Call Now ✓
  2. Personal story → "Our Story" (how/why you got into the trade — the "Experience" E) ✓
  3. Author bio box → "Meet the Owner/Team" ✓
  4. Social media links → "Connect With Us" (+ the smart "only link profiles you maintain" warning) ✓
  5. Multimedia (video ideal, images minimum) → "Video Introduction" + image/headshot space ✓
  6. GBP linking conditional → "local → homepage; service-area → About acceptable" — **matches 8.3 item 6 exactly** ✓
  - **Plus it closes 8.3's noted omission:** 8.3 flagged that specific credentials/licenses weren't on the checklist; Prompt 7 adds a dedicated "Credentials & Trust" section (license #, insurance, certs, years).
- 🔄 **Technical Foundation / Contact** — NAP, large click-to-call, mailto, ContactPage/LocalBusiness schema all operationalize the documented rules.
- ↔️ **Pairs with 1.2 AI Readiness NAP & Authority Check** (as 8.3 notes): 1.2 audits external authority; Prompt 7 builds the on-site authority. Complementary.
- 🆕 The two-column contact layout, form-handler note, and the credentials section beyond 8.3.

**Role in the sequence:**
- **Step 7 — the trust/credibility pages.** With this, every page in the architecture is built. Only the site-wide technical pass (Prompt 8) remains.

---

# Prompt 8 — Technical SEO Implementation

**Role assigned:** "Senior web developer and technical SEO specialist." Final technical pass + verification + index-readiness. **This is a verify-and-fix audit, not a content/build step** — it reviews what Prompts 1–7 produced.

**What it does / output (10 parts):**
1. **sitemap.xml** — all pages, current `lastmod`, priority tiers (home 1.0; category/core 0.8; services 0.7; child 0.6; about/contact 0.5), changefreq monthly (weekly homepage); verify count = PAGE COUNT SUMMARY.
2. **robots.txt** — allow all, point to sitemap, block admin/api.
3. **Schema verification** — per-page schema check; homepage gets a category-specific LocalBusiness type + priceRange "$$" + openingHours + sameAs; About adds Person schema.
4. **Meta tag verification** — unique titles **under 60 chars**, unique meta descriptions under 160, exactly one H1/page, clean H1→H2→H3 hierarchy.
5. **Internal link audit** — match the INTERNAL LINKING MAP; no broken links, no orphans, clean URLs, ScrollToTop working.
6. **Mobile** — tel: click-to-call, hamburger, floating Call Now, 44×44 touch targets, no horizontal scroll.
7. **Page speed** — image compression/WebP/dimensions/lazy/alt, minified CSS+JS, **Lighthouse 80+ mobile**.
8. **404 page** — custom, on-brand, helpful.
9. **Additional** — self-referencing canonical tags, favicon, Open Graph tags, `<html lang="en">`, viewport meta.
10. **Final verification checklist** + output report (schema errors fixed, broken links fixed, missing elements, page-count verification, recommendations).

**Usage notes:**
- This is the **verification step** your own methodology always wants before calling a build done — and it's genuinely comprehensive on *on-page* technical SEO. Run it as a real audit, not a rubber stamp (see the title-length point below).
- ⚠️ **Its own criteria expose the course's earlier drift.** Part 4 demands titles "under 60 characters" and "consistent format across site." But Prompts 3–7 generated **five different hardcoded qualifiers** and a homepage title (~62 chars) that **breaks the 60-char rule.** Run honestly, Prompt 8 *should flag its own predecessors.* The course never acknowledges the contradiction — so treat Prompt 8 as the place to standardize qualifiers and trim the homepage title.
- ⚠️ **Omits BreadcrumbList schema.** Your AI Agent TECHNICAL FOUNDATION requires breadcrumb schema on category/service pages; Prompt 8's schema list (LocalBusiness, Service, ContactPage, Person) doesn't include it. Add manually for parity.
- ⚠️ **Doesn't invoke the validator tool.** Part 3 says "valid JSON-LD" but never points at validator.schema.org. Validate there yourself.

✅ **Schema-dedup — RESOLVED, and done correctly.** Part 3 mandates schema "with consistent business information across all pages" using **"the same @id reference for LocalBusiness throughout,"** with all Service schemas referencing that LocalBusiness as `provider`. That's the proper JSON-LD pattern for a single business entity — it prevents the duplicate-entity problem the per-page injection (Prompts 3–7) could otherwise cause. So the build prompts scatter schema; Prompt 8 unifies it under one @id. No double-add concern.

🔴 **Lovable SPA crawlability — NOT solved here. This is the most important takeaway of the finale.**
- Everything in Prompt 8 (sitemap, robots, canonical, meta, schema, OG) **assumes the page content already exists in the HTML.** None of the ten parts address **server-side rendering, prerendering, or static generation.**
- But Prompt 1 established this is a **React SPA with client-side routing** (the mandated ScrollToTop-on-route-change). Client-rendered SPAs can serve near-empty initial HTML to crawlers — Google renders JS with delay/budget limits, and Bing + AI crawlers (which this methodology explicitly targets) handle it worse.
- **Strong inference:** the actual "make the SPA crawlable" fix lives in the **"Lovable HTML: NEEDED to Get Ranked" lesson** — which sits *outside* the numbered prompt sequence and which you haven't pasted yet. That lesson's title is the tell. **Prompt 8 is necessary but not sufficient: without the rendering fix, all 8 prompts can produce a beautiful site that still doesn't rank because crawlers can't see the content.** Paste the Lovable HTML lesson to close this loop — it's arguably the single highest-stakes piece of the course.

**Cross-references & overlaps:**
- 🔄 **TECHNICAL FOUNDATION REQUIREMENTS (AI Agent Prompt) + Technical Foundation (Complete Playbook).** Prompt 8 implements all of it — schema, NAP consistency, tel: links, Core Web Vitals, crawlability/robots — and goes **further** than your documented spec by adding sitemap.xml, canonical tags, Open Graph, a custom 404, favicon, and a Lighthouse target. Only gap vs. spec: BreadcrumbList schema (above).
- 🔄 **Tool: Schema Markup Validator** (Resources) — corresponds to Part 3, though Prompt 8 doesn't name the tool.
- 🔄 **AI Agent "Site Map" output** → Prompt 8's sitemap.xml is the literal XML implementation of that planned structure.
- 🆕 sitemap.xml file generation, OG tags, custom 404, canonical/favicon/lang/viewport as an explicit checklist — and the unaddressed SPA-rendering gap.

**Role in the sequence:**
- **Step 8 — index-readiness audit.** Closes the build. ⚠️ But true rank-readiness for a Lovable SPA depends on the separate Lovable HTML lesson, not this prompt.

---

# Cross-Reference Map (running)

Live tally of how this course relates to the main notes. **All entries are _candidate_ overlaps to confirm or rule out as each prompt comes in** — nothing verified yet.

| This course | Main-notes asset | Section | Likely relationship |
|---|---|---|---|
| Prompt 0 (Planning) | AI Agent Prompt — Local Business Website Builder | Main notes | 🔄 **CONFIRMED.** Modular twin = the AI Agent's Site Map output, minus strategy intake & Locations/Supporting Content, plus a "General Services" bucket. "Core Services" = AI Agent's "Critical Services." |
| Prompt 0 | 8.1 Local Site Structure Blueprint | Prompt Catalog | 🔄 **CONFIRMED.** Same architecture + linking logic; Prompt 0 adds State Abbrev to keyword + a URL-slug convention; omits Supporting Content/Locations. |
| Prompt 0 | 3.4 GBP Categories / P&T #3 | Catalog / P&T | ⬆️ **Upstream prerequisite**, not overlap — Prompt 0 consumes its output. |
| Prompt 0 | 4.6 Service Entity Research / P&T #4 | Catalog / P&T | ⬆️ **Upstream prerequisite**, not overlap — Prompt 0 consumes its service list. |
| Prompt 0 | 1.4 Core 30 Structure Checker / P&T #5 | Catalog / P&T | ↔️ **Inverse tool** — 1.4 audits existing sites; Prompt 0 plans new builds. Complementary. |
| Lovable HTML lesson | Technical Foundation / crawlability | Playbook + AI Agent Prompt | ✅ **CONFIRMED — closes the Prompt 8 SPA gap.** Pre-render + 200-redirect = only non-redundant fixes; rest overlaps Prompt 8. 🆕 CSR/pre-render mechanics. |
| Prompt 1 (Skeleton) | — (no prior asset) | — | 🆕 **CONFIRMED net-new.** Front-end scaffolding (routes, design tokens, sticky header, floating call button, hamburger, ScrollToTop). No equivalent in main notes. |
| Prompt 1 | Technical Foundation / Tech Requirements | Playbook + AI Agent Prompt | 🔄 **CONFIRMED.** Header/footer NAP, `tel:` click-to-call, mobile-first, semantic HTML5 operationalize the documented rules at skeleton stage. |
| Prompt 2 (GBP LP Content) | 2.4 Goal Completion Rewrite / P&T #2 | Catalog / P&T | 🔄 **CONFIRMED.** Same goal-completion root; Prompt 2 scales the principle across the whole homepage vs. 2.4's single <50-word block. |
| Prompt 2 | 2.1 Local SEO Content Writer / P&T #1 | Catalog / P&T | 🔄 **CONFIRMED — alternative approach.** 2.1 = length/keyword-driven (+ banned-words list); Prompt 2 = conversion/structured (no word target, **no banned-words list**). |
| Prompt 2 | Homepage (GBP LP) spec | Playbook + AI Agent Prompt | 🔄 **CONFIRMED — content layer only.** Matches tone/H1/sections; schema, embeds, NAP, <50-word fold, 5th-grade level handled by Prompts 1/3/8. |
| Prompt 2 | 2.5 Determine Searcher Intent | Catalog | 🔄 Same Goal-Completion framework; run 2.5 first to sharpen above-the-fold emphasis. |
| Prompt 3 (GBP LP Build Out) | GBP Landing Page Quick Hits | GBP Optimization Materials | 🔄 **CONFIRMED — satisfies all 9 items.** Cleanest 1:1 map in the course. |
| Prompt 3 | Homepage spec | AI Agent Prompt + Playbook | 🔄 **CONFIRMED — execution layer.** Omits the required **GBP map embed**; adds Zehl-derived section order + hardcoded emergency qualifiers. |
| Prompt 3 | Goal Completion (2.4 / 2.5) | Catalog / P&T | 🔄 Applied to section ORDER (proof first, education last), not just copy. |
| Prompt 3 | — (layout order) | — | 🆕 11-section conversion order, hero image gen, sticky mobile CTA bar, lead-form section. |
| Prompt 4 (Secondary Category) | Secondary Category Pages spec | Playbook + AI Agent Prompt | 🔄 **CONFIRMED — clean implementation** + adds fixed 4-H2 structure, word count, grid, schema. |
| Prompt 4 | Internal Linking Mirror / Rules | Module 3 + AI Agent Prompt | 🔄 **CONFIRMED.** DOWN to every child service + UP to homepage; clean URLs, no `#`. |
| Prompt 4 | 2.1 Local SEO Content Writer / P&T #1 | Catalog / P&T | 🔄 ≈ 2.1's category-page adaptation fused with build-out (dual-audience, local refs). |
| Prompt 4 | CONTENT GENERATION RULES | AI Agent Prompt | 🔄 Dual-audience + 5th-grade + avoid-words — but avoid list is shorter/divergent (15 words). |
| Prompt 4 | Service Pages tone rule | AI Agent Prompt | ⚠️ **TENSION** — spec says vary tone by service type (high-ticket → investment framing); course hardcodes emergency framing. Critical for Prompt 5/6. |
| Prompt 5 (Core Service) | Service Pages spec / 2.1 / Module 3.3 | Playbook / Catalog / Main | 🔄 **CONFIRMED — crisis-tuned twin of Prompt 4.** 🔴 Overrides spec's high-ticket "investment framing" with hardcoded urgency. |
| Prompt 6 (Service) | Module 3 Core 30 / 1.4 Checker / 8.1 Blueprint | Main / Catalog | 🔄 **CONFIRMED — the Core 30 build engine.** Builds the GBP Service Pages layer + `/services` hub. **Omits the blueprint's Supporting Content branch.** |
| Prompt 7 (About/Contact) | 8.3 E-E-A-T About Page Checklist | Catalog | 🔄 **CONFIRMED — near-complete implementation** (all 6 items + closes 8.3's credentials omission). Cleanest asset→template map in the course. |
| Prompt 7 | Technical Foundation / 1.2 NAP & Authority | Playbook / Catalog | 🔄 Contact NAP/click-to-call/schema; About builds on-site authority (pairs with 1.2's external audit). |
| Prompt 8 (Technical SEO) | Technical Foundation / Schema Validator | Playbook / AI Agent / Resources | 🔄 **CONFIRMED — implements + exceeds** the spec (adds sitemap, canonical, OG, 404). ✅ Schema-dedup via single @id. 🔴 Does NOT solve SPA rendering; omits BreadcrumbList. |

_As prompts are confirmed, update the relationship column to ✅ / 🔄 / 🆕 and link to the specific section above._

---

# Workflow Logic — The Build Sequence

*To be built up as prompts arrive. Maps how output flows prompt-to-prompt and where dependencies sit.*

**Confirmed shape (from lesson titles):** The sequence builds the site page-type by page-type, in the same priority order as the main notes' architecture — GBP landing page first, then secondary category pages, then service pages, then about/contact, then a technical pass. This validates the build-order hypothesis from the skeleton draft.

**Notable structural patterns to watch:**
1. **Scaffold-everything-first, fill-later** — ✅ **CONFIRMED (Prompts 1+4).** Full site built as empty routes up front (Prompt 1); content poured in page-type by page-type. ⭐ **Confirmed asymmetry: the homepage is the ONLY page type with a dedicated content prompt (Prompt 2) + build prompt (Prompt 3). Every other page type (category in Prompt 4, services in 5–6, about/contact in 7) generates content INLINE during a single combined build-out prompt** that takes only the Prompt 0 block as input. ⚠️ Methodological tension to keep in mind: the main notes preach phased, rank-map-gated expansion and warn against building too fast / thin content; this course front-loads the entire structure. Reconcile by sequencing — fill + publish content before crawlers see placeholder routes.
2. **"Core Service" (Prompt 5) vs. "Service" (Prompt 6)** — ✅ **RESOLVED by Prompt 0.** Prompt 0's hierarchy defines **Core Services** as high-value services that get prominent homepage placement and link directly from the homepage (= the AI Agent Prompt's "Critical Services"), while ordinary **Child Services** sit under categories/core services. So Prompt 5 builds the homepage-linked core services; Prompt 6 builds the child/general service pages (the Core 30 volume).
3. **No location-page prompt** — consistent with location pages being Phase 4 (after 30–40% green) in the main notes, deliberately out of scope for the initial build.
4. **Lovable as the build surface** — the "content" prompts generate copy; the "build out" prompts presumably produce Lovable-ready output. The Lovable HTML lesson is the bridge to ranking-readiness.

**Sequence diagram (fill in dependencies as confirmed):**

```
Prompt 0 (Plan) ── the single source of truth; pasted into every prompt below
   │
Prompt 1 (Skeleton) ── empty routed React SPA shell (consumes Prompt 0)
   │
Prompt 2 (GBP LP Content) ──> Prompt 3 (GBP LP Build Out)   [only page type with a content/build split]
   │
Prompt 4 (Secondary Category)  ┐
Prompt 5 (Core Service)        │  combined content+build; each consumes Prompt 0 only
Prompt 6 (Service + /services) │  (Prompt 6 = Core 30 volume)
Prompt 7 (About + Contact)     ┘
   │
Prompt 8 (Technical SEO audit) ── sitemap/robots/schema-unify/meta/links/mobile/speed/404
   │
[Lovable HTML lesson] ── SPA rendering fix REQUIRED for crawlability (outside the sequence)
```

**Dependency notes:**
- Prompt 0 is pasted into all of 1–8 (and Prompt 2 into Prompt 3). It is the only cross-prompt data carrier.
- Prompts 4–7 do not depend on each other — they each read only the Prompt 0 block, so they can run in any order.
- Prompt 8 audits the cumulative output but consumes only Prompt 0 for its checklist.
- The Lovable HTML fix is a parallel dependency, not a sequence step — it must be applied for the build to rank.

---

# Open Questions / To Verify

- ~~Is this course the modular version of the AI Agent Prompt?~~ → ✅ **Largely confirmed by Prompt 0.** Prompt 0 maps onto the AI Agent Prompt's Site Map output, minus the strategic diagnostic layer. This course is the modular *build* path; the AI Agent Prompt is the all-in-one *strategist + spec*.
- ~~Does Prompt 0 run GBP discovery or assume it's done?~~ → ✅ **Resolved.** Prompt 0 *consumes* finalized GBP categories + services as inputs; discovery (3.4 / 4.6) is upstream.
- ~~Confirm "Core Service" vs. "Service" split.~~ → ✅ **Resolved** (see Workflow Logic #2).
- ~~Title-tag drift~~ → ✅ **RESOLVED in Prompt 3.** Real `<title>` = `[TARGET KEYWORD] | 24/7 Emergency Service | [BUSINESS NAME]` → state abbrev **retained**. Diverges from your `Primary Category + City | Brand` (<60 char) convention three ways: + state abbrev, + hardcoded middle qualifier, runs long (~62 chars). Pick a standard for your own builds.
- 🔴 **Tone-by-service-type tension — NOW DECISIVE (Prompt 5).** Core service pages hardcode crisis/urgency framing ("crisis/urgent situation," "disruption to their life," "isn't a wait-and-see problem," "Same-Day Service Available"). The AI Agent spec says high-ticket services get **investment framing**, not urgency. **For Crowley's countertops this is backwards.** Surgical fix: keep Prompt 5's decision structure ("Our Options," "What to Expect," repair-vs-replacement), strip the urgency/same-day language, swap in investment framing + budget guidance (~$5k small / ~$8k larger kitchen).
- ⚠️ **"No specific prices" conflicts with your Crowley's preference (NEW).** Prompt 6's Cost-in-[City] section forbids concrete prices; your standing Crowley's copy preference is to **include** budget expectations (~$5k small / ~$8k larger kitchen). Override the course default for Crowley's.
- ⚠️ **Supporting Content layer omitted (NEW).** 8.1 Blueprint's Core 30 includes 2 supporting-content pieces per high-priority service; this course builds service pages but no supporting-content branch. Separate work if you want the full blueprint.
- ⚠️ **Banned-words inconsistency (CONFIRMED across 5 prompts):** P2=0, P4=15, P5=16, P6=15 words; none match your canonical list. **Paste your full avoid-words list into every content prompt.**
- ⚠️ **Title qualifier drift (FIVE-way):** Emergency (home) / Complete Service List (services hub) / Fast Reliable (category) / Same-Day Available (core) / Fast Professional (child). All hardcoded; edit per business.
- ~~Are TRUST SIGNALS / LOCAL ISSUES from Prompt 0 reused downstream?~~ → ✅ **RESOLVED.** Prompt 4 references **LOCAL ISSUES, SERVICE AREAS, and TRUST SIGNALS** from the Prompt 0 block directly. ⚠️ **New coherence risk:** category pages use Prompt 0's TRUST SIGNALS (possibly AI-guessed) while the homepage uses Prompt 2's real differentiators — **they can disagree.** Reconcile the Prompt 0 block to hold real signals before running Prompt 4.
- ⚠️ **Input-chain gap (NEW):** Prompt 4 expects "HOMEPAGE ANCHOR TEXT OPTIONS" from the architecture, but Prompt 0's output template doesn't clearly produce it. Add anchor-text options to your Prompt 0 block.
- ⚠️ **Tone-by-service-type:** see the 🔴 decisive item above (resolved/escalated at Prompt 5).
- ~~Schema dedup~~ → ✅ **RESOLVED in Prompt 8.** Build prompts (3–7) scatter per-page schema; Prompt 8 unifies it under a **single shared @id for LocalBusiness** with all Service schemas referencing it as `provider`. Correct JSON-LD pattern — no double-add concern. (Gap: Prompt 8 omits BreadcrumbList schema the AI Agent spec wants; add manually.)
- ~~Where does Lovable crawlability get solved?~~ → ✅ **RESOLVED.** Lovable = CSR React/Vite → blank `<div id="root">` shell to bots. Fix = pre-rendering (Lovable's native **Discoverability** feature, or LovableHTML/Hado/static deploy) **+ host 200-redirect of deep routes to index.html.** Those two are the only items Prompt 8 doesn't already cover. ⚠️ The chat prompt alone ≠ true SSR — the fix is at the deploy/host layer; verify the bot's-eye HTML before trusting rankings.
- ⚠️ **Locations-hub mismatch:** Prompt 3 homepage links to `/locations/` + location pages the architecture never built (Phase 4 deferral). Hold or condition those links.
- ⚠️ **GBP map embed:** present on `/contact` (Prompt 7) but **still absent from the homepage**, where the AI Agent spec wants it for a local business. Contact map ≠ homepage requirement. Add to homepage manually for parity.
- ⚠️ **Hardcoded `© 2025`** in the Prompt 1 footer — update to current year.
- What exactly is the Lovable ranking problem the "NEEDED to Get Ranked" lesson fixes? (Default Lovable HTML crawlability?)
- Are any of Prompts 1–8 verbatim copies of existing cataloged prompts vs. new Lovable-specific variants?

---

## References

[1] [Caleb Ulku, “Core 30 Sample Website Overview for Plumber in Gary, Indiana,” *AI SEO Mastery*, Classroom Overview video](https://www.skool.com/ai-seo-mastery/classroom/f8367d03?md=e8e9c2b0c6bd4f9094fe2aa34dba4934)

