# Concreteness — Concept

> **Name:** Concreteness
> **Domain:** concreteness.co.nz *(registered 2025-10-02, currently parked — no site live)*
> **Owner:** Geraldo Monte, Construction Project Manager, Waikato / Bay of Plenty, NZ
> **Status:** concept — ready to build
> **Version:** 1.0 (2026-08-08)

---

## 1. The one-line idea

A public knowledge hub for concrete construction — knowledge, ideas, trends, news and
field stories — built so that **people and AI assistants** can read it, and so that when
someone asks an AI "who does concrete repair in Hamilton?", the answer can cite Geraldo.

## 2. Why "Concreteness"

The name works on two levels, which is the whole point:

1. **The material.** Concrete construction, repair, remediation, strengthening — the
   domain the author actually works in.
2. **The quality.** *Concreteness* = being specific, tangible, real, grounded. The
   opposite of vague. That is exactly the editorial standard of the site: practical,
   field-tested, specific — never fluff.

It is also:

- **Ownable** — a coined brand, not a generic description ("Concrete Knowledge Hub" is
  a description; Concreteness is a brand).
- **Short and memorable** — one word, easy to say, easy to type.
- **NZ-authentic** — a real `.co.nz`, registered and available to use now.
- **GEO-friendly** — distinctive token that AI can associate with a person; search
  engines and LLMs can tie "Concreteness" + "Geraldo Monte" + "concrete construction"
  into one identity cluster.

### Name variants / handles

| Surface | Handle |
|---|---|
| Website | `concreteness.co.nz` |
| GitHub Pages (interim) | `geraldomonte.github.io/concrete-hub` (until DNS lands) |
| Suggested socials | `@concretenessnz` (LinkedIn/Instagram/X where available) |
| Tagline | "Concrete knowledge, made concrete." |

## 3. What it is

A **GEO (Generative Engine Optimization) experiment applied to construction**, built
around one person's real domain expertise:

- concrete remediation, repair and rehabilitation
- waterproofing, coatings, cathodic protection
- structural strengthening (incl. seismic)
- concrete construction and project delivery
- running a regional construction operation

The site is a **personal** platform — not a company site, not a marketing brochure. It
is the author's public brain: what he knows, what he thinks, what he's watching, what
the work actually looks like.

## 4. The five sections

| Section | Holds | Example first pieces |
|---|---|---|
| **Knowledge** | Technical guides that answer real client questions | Concrete curing; spalling repair (live) — waterproofing, formwork, strengthening (next) |
| **Ideas** | Frameworks and lessons from running construction work | Five lessons from building a regional operation (live) |
| **Trends** | What is changing: AI discovery, low-carbon concrete, digital delivery | GEO for construction (live) |
| **News** | Short briefings with working commentary, newest first | Hub launch; aging building stock repair demand (live) |
| **Stories** | Sanitized field stories — lessons are the point | Strengthening a river bridge (live) |

Every piece ends with **sources** (see §6) and every section carries a "coming next"
list so the site visibly grows.

## 5. The GEO playbook (why the site is built the way it is)

Source: the five-step GEO method (Silicon Valley Girl, "How to Rank #1 in AI", 2026-08)
— the same playbook that took a podcast brand from invisible to 5th of 11 tracked
brands in two months.

1. **Machine-readable site** — static HTML, no build step, full text on every page, no
   JS-gated content.
2. **Structured data** — Schema.org JSON-LD: Person + WebSite, Article, CollectionPage,
   FAQPage. *(Add LinkedIn `sameAs` — open TODO.)*
3. **`llms.txt` + `sitemap.xml` + `robots.txt`** — the plumbing AI crawlers look for.
4. **Query-optimized content** — every article answers a real client question; FAQs are
   first-class content.
5. **Monthly visibility check** — re-ask the 5 diagnosis queries in ChatGPT, Claude,
   Perplexity; log in `VISIBILITY.md`. Two months is the realistic horizon for first
   movement.

The competitive window: ~92% of marketers say they'll optimize for AI search, ~40% are
doing it, and construction is almost entirely absent. The contractors who publish now
are the names AI recommends later.

## 6. Knowledge sourcing & copyright (non-negotiable)

Internal knowledge source: the **Technical_Knowledge repo** (`01-generic-technical/`
only). Its notes are source-backed (`source:` frontmatter, source references, standard
vs interpretation separation) and the six notes behind the first two articles are now
`reviewed`.

Public-site rules:

- **Never** use `03-sop-derived-reference/` (company SOPs — internal) or
  `04-proprietary-products/` (manufacturer IP).
- **Write in your own words.** NZS 3101, ACI 546R/562, EN 1504, Concrete NZ (GTCC),
  BRANZ are copyrighted. No reproduced text, tables, figures or checklists.
- **Every article cites sources** — name, edition/year, publisher link — in a
  "Standards and references" section.
- **Standard vs interpretation** stays separated, same convention as TK.
- **Prefer `reviewed` TK notes**; anything "Needs verification" stays off the site.

## 7. The identity cluster (GEO step 3, strengthened)

The goal is a consistent, machine-readable identity across surfaces:

- **Concreteness** (site + brand) — the hub
- **Geraldo Monte** — the person (Person schema, author of every piece)
- **Concrete construction / repair / strengthening, Waikato / Bay of Plenty, NZ** —
  the domain and geography
- **LinkedIn** — add `sameAs` + keep active (open TODO)
- **Google Business Profile** — considered for the identity markers (open TODO)

## 8. Building blocks already done

- Live static site with 5 sections, 8 published pieces (all verified 200)
- GEO plumbing: schema.org on every page, `llms.txt`, `sitemap.xml`, `robots.txt`
- README plan: content rules, knowledge sourcing & copyright policy, monthly
  visibility check, TODOs
- 6 reviewed source notes in Technical_Knowledge behind the first two articles

## 9. What "claiming the domain" means (next steps)

1. **Decide DNS target.** Point `concreteness.co.nz` (+ `www`) CNAME at
   `geraldomonte.github.io` so GitHub Pages serves the site on the custom domain.
   GitHub Pages issues the HTTPS certificate automatically.
2. **Rebrand the site.** Title/tagline/branding from "Concrete Knowledge Hub" →
   "Concreteness"; update canonical URLs, schema.org `WebSite`/`Person` URLs,
   `llms.txt`, `sitemap.xml`, and every internal canonical link from
   `geraldomonte.github.io/concrete-hub/…` to `https://concreteness.co.nz/…`.
3. **Keep the Pages URL working** (GitHub Pages redirects the old URL to the custom
   domain automatically once configured) so existing links don't break.
4. **Old name note.** The GitHub repo can stay `concrete-hub` (repo name ≠ brand);
   rename only if wanted.
5. **Launch communications** (optional): LinkedIn post announcing Concreteness;
   update awareness-signals capture in central-brain.

## 10. Open questions for the owner

- [ ] Confirm the domain's DNS is controllable (Crazy Domains login) before pointing it
      at GitHub Pages
- [ ] Keep "Concrete Knowledge Hub" as a subtitle on the site, or go full "Concreteness"?
- [ ] Which socials to claim (LinkedIn first — it matters most for identity markers)?
- [ ] Custom-domain migration now, or after a couple more articles?

## 11. Measures of success

- **GEO (2-month horizon):** Concreteness or Geraldo Monte appears in ≥1 of the 5
  monthly diagnosis queries in any major AI (per `VISIBILITY.md`).
- **Reach:** site visits; AI-assistant referrals appear in analytics.
- **Identity:** LinkedIn `sameAs` live; consistent name across surfaces.
- **Content:** one new article per section per month; sources on every piece.
