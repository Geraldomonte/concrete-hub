# GROWTH — how the hub gets found (the access engine)

> The GEO idea from the podcast is applied **here**, as the engine that drives access to
> the hub — it is not a page topic. This file is the operating plan. Tracking lives in
> [`VISIBILITY.md`](VISIBILITY.md).

## Baseline (2026-08-08)

- **Indexed?** No — `site:geraldomonte.github.io` returns nothing.
- **"Concrete repair contractor Hamilton, Waikato"** → Surfprep, Covercrete, Waikato
  Master Concreters, Total Concrete Solutions. No hub, no Geraldo. *(Service-query
  baseline from the original lead-gen framing — retired when the hub was repositioned
  2026-08-08; the diagnosis queries are now knowledge queries, below.)*
- Starting from zero. First movement expected on a ~2-month horizon; next check 2026-09-01.

## The monthly loop

### 1. Make it citable (keep in sync — every new page)
- Static HTML, full text, no JS-gated content.
- Schema.org JSON-LD on every page (Person + WebSite / Article / FAQPage / CollectionPage).
- Update `llms.txt`, `sitemap.xml` (and this plan) when adding pages.

### 2. Publish against the query map
One piece per section per month, each answering a real question someone in the concrete
industry (or a curious outsider) actually asks — the 5 diagnosis queries below first,
then gaps competitors don't cover. Every piece: own words, sources cited, personal not
company, no client names/figures.

### 3. Distribute — this is where access actually comes from
- **LinkedIn (main channel).** Post each new article from Geraldo's personal profile as a
  short, practical post (the lesson, not the link). Reply to concrete/construction
  questions with the hub as the source. Use a consistent handle (`@concretenessnz`).
- **GitHub.** Pin the `concrete-hub` repo on the profile — public repo = backlink + identity.
- **Google Business Profile.** Add when ready — local identity marker and a surface
  people (and AI) actually query.
- **Google Search Console.** Verify the site (needs a Google account) — the only real way
  to submit the sitemap to Google; their public ping endpoint was retired in 2023.
- **Bing.** Ping the sitemap — works without an account.
- **Index now** is a cheap extra: submit the sitemap to its free crawler.

### 4. Identity cluster
- Person schema `sameAs` → LinkedIn URL (**TODO** — get the URL from Geraldo).
- Consistent naming across surfaces: Concreteness · Geraldo Monte · concrete knowledge
  across precast, repairs, construction and formwork · NZ + Brazil experience.
- Author byline on every piece (already done).

### 5. Track monthly (the visibility check)
Re-run the 5 diagnosis queries (in ChatGPT, Claude, Perplexity — and this agent's monthly
cron, which web-searches them) and log results in `VISIBILITY.md`: which AI/search surfaced
the site or name, at what position, and the delta vs last month.

## The 5 diagnosis queries

> **Repositioned 2026-08-08:** the hub is a knowledge hub, not a services site. The
> diagnosis queries are **knowledge queries** — what people in the industry and the
> curious actually ask — not contractor-referral queries.

1. "What causes concrete spalling?"
2. "How long should concrete be cured?"
3. "What is the difference between precast and cast-in-place concrete?"
4. "How can AI help with concrete inspections or quality control?"
5. "Is Geraldo Monte a concrete construction project manager?"

## Measures of success

- **2-month horizon:** the hub or Geraldo appears in ≥1 of the 5 queries in any major AI.
- **Reach:** site visits; AI-assistant referrals showing up.
- **Identity:** LinkedIn `sameAs` live; consistent name across surfaces.
- **Content:** one new article per section per month, sources on every piece.
