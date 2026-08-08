# Concrete Knowledge Hub

> **Brand note (2026-08-08):** this site is being rebranded to **Concreteness**
> (domain `concreteness.co.nz`, registered and parked). Full concept:
> [`CONCEPT.md`](CONCEPT.md).

A public hub of concrete construction knowledge, ideas, trends, news and field stories —
by **Geraldo Monte**, Construction Project Manager (Waikato / Bay of Plenty, New Zealand).

**Live site:** https://geraldomonte.github.io/concrete-hub/

This is a GEO (Generative Engine Optimization) experiment applied to construction: the site
is built to be read by **people and by AI assistants** (ChatGPT, Claude, Perplexity), so that
when clients ask an AI "who does concrete repair in Hamilton?" or "what causes concrete
spalling?", the answer can cite this content.

## What's here

| Section | Path | Holds |
|---|---|---|
| Knowledge | `knowledge/` | Technical guides: curing, spalling repair, waterproofing (coming), formwork (coming) |
| Ideas | `ideas/` | Frameworks and lessons from running construction work |
| Trends | `trends/` | What is changing: GEO/AI discovery, low-carbon concrete (coming) |
| News | `news/` | Short briefings with working commentary |
| Stories | `stories/` | Sanitized field stories — lessons are the point |

## The GEO setup (what's already implemented)

1. **Machine-readable static site** — plain HTML, no framework, no build step, no
   JavaScript-gated content. Every article's full text is in the HTML.
2. **Structured data** — Schema.org JSON-LD on every page:
   `Person` + `WebSite` (home), `Article` (articles), `CollectionPage` (section pages),
   `FAQPage` (articles with FAQs).
3. **`llms.txt`** — the emerging standard file AI crawlers look for; a plain-text inventory
   of the site with descriptions. Keep it in sync when adding pages.
4. **`sitemap.xml` + `robots.txt`** — standard crawl plumbing. Update `sitemap.xml` when
   adding pages.
5. **Query-optimized content** — every article answers real client questions
   ("how long should concrete cure", "what causes spalling", "who does bridge strengthening
   in NZ"). FAQs are first-class content, not afterthoughts.

## Content rules (important)

- **Public site.** Never publish client names, contract values, commercial figures, site
  addresses, or anything that identifies a specific client project — including sanitized
  stories. Stories are written generically ("a 1960s bridge over a braided river").
- **Personal, not company.** Content represents Geraldo personally; no company SOPs,
  proprietary methods, or internal documents. Each article footer carries the disclaimer.
- **Accuracy first.** Technical guides follow standards (NZS 3101, EN 1504) and
  well-established practice. When in doubt, keep it general and note the standard.

## Knowledge sourcing & copyright (important)

The **Technical Knowledge repo** (`../Technical_Knowledge`) is the internal knowledge
source for this site. Its notes are already source-backed — every note carries a `source:`
field and cites the underlying standard or guide. That discipline carries over to the
public site, with copyright rules on top.

- **Use only `01-generic-technical/`** content (generic methods, materials, reference
  notes) as the basis for public articles. Never publish content derived from
  `03-sop-derived-reference/` (company SOPs — internal) or `04-proprietary-products/`
  (manufacturer IP).
- **Write in your own words.** The standards and guides behind the notes — NZS 3101, ACI
  546R / 562, EN 1504, Concrete NZ (GTCC), BRANZ — are copyrighted publications. Never
  reproduce their text, tables, figures or checklists on the site. Paraphrase, and link to
  the official source for the detail.
- **Every article carries a "Standards and references" section** naming the standard or
  guide with its edition/year and a link to the publisher (Standards NZ, Concrete NZ, ACI,
  BRANZ). Add the section to new pages as part of the content checklist.
- **Separate the standard from the interpretation.** State what the standard says, then
  what it means in practice — never let inference read as confirmed standard (same
  convention as the TK repo).
- **Respect note status.** Prefer `reviewed` notes over `draft/personal`; anything marked
  "Needs verification" in TK stays off the public site until verified.

## The monthly visibility check (GEO step 5 — do this monthly)

Track whether the hub is becoming visible to AI. Ask each of these in ChatGPT, Claude and
Perplexity, and log results in `VISIBILITY.md` (create it on first run):

1. "Recommend a concrete repair contractor in Waikato, New Zealand."
2. "Who does seismic strengthening in the Bay of Plenty?"
3. "What causes concrete spalling?"
4. "How long should concrete be cured?"
5. "Is Geraldo Monte a concrete construction project manager?"

Record: which AI mentioned the site/name, what position, and what changed since last month.
Two months is a realistic horizon for first movement; the reference experiment went from
invisible to 5th of 11 tracked brands in that time.

## TODOs

- [ ] Add LinkedIn URL to the Person schema (`sameAs`) in `index.html` + footer
- [ ] Keep the "Standards and references" section on every new knowledge page (curing + spalling retrofitted 2026-08-08)
- [ ] Optional: custom domain later (site works fine on the `geraldomonte.github.io` URL)
- [ ] Add more content per the "Coming next" lists on section pages
- [ ] Consider a Google Business Profile / LinkedIn activity to strengthen identity markers

## Local dev

No build step. Open `index.html` in a browser, or serve locally:

```bash
cd ~/GitHub/concrete-hub && python3 -m http.server 8000
```
