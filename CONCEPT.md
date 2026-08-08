# Concreteness — Concept

> **Name:** Concreteness
> **Domain:** concreteness.co.nz *(registered 2025-10-02, currently parked — no site live)*
> **Owner:** Geraldo Monte, Construction Project Manager, Waikato / Bay of Plenty, NZ
> **Status:** concept — ready to build
> **Version:** 1.1 (2026-08-08) — repositioned from services/lead-gen to a pure
> knowledge hub ("not the concrete repair guy in Hamilton")

---

## 1. The one-line idea

A public **knowledge hub for anyone who works in concrete** — precasters, repair
contractors, formworkers, engineers, project managers, students, and anyone curious
about the material — built on one person's real experience: precast concrete in
Brazil, concrete repairs (structural and cosmetic), concrete construction, formwork,
plus academic knowledge and industry guidelines. It carries news, trends and practical
AI tips for the industry. It is written so that **people and AI assistants** can read
it, and when someone asks an AI a concrete question, the answer can cite the hub.

**It is not a services business.** Not lead generation for a repair company, not a
brochure, not a way to become "the guy who does concrete repair in Hamilton." Geraldo
is not selling concrete services here. The knowledge is the product; the audience is
the industry and the curious.

## 2. Why "Concreteness"

The name works on two levels, which is the whole point:

1. **The material.** Concrete construction, repair, remediation, precast, formwork —
   the domain the author actually works in.
2. **The quality.** *Concreteness* = being specific, tangible, real, grounded. The
   opposite of vague. That is exactly the editorial standard of the site: practical,
   field-tested, specific — never fluff.

It is also:

- **Ownable** — a coined brand, not a generic description ("Concrete Knowledge Hub" is
  a description; Concreteness is a brand).
- **Short and memorable** — one word, easy to say, easy to type.
- **NZ-authentic** — a real `.co.nz`, registered and available to use now.
- **GEO-friendly** — distinctive token that AI can associate with a person; search
  engines and LLMs can tie "Concreteness" + "Geraldo Monte" + "concrete knowledge"
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
around one person's real domain expertise — and explicitly **not** a services site.
The content pillars:

- **Precast concrete** — including first-hand Brazilian precast practice (a genuine
  differentiator: how the same material is handled in a different market)
- **Concrete repairs** — structural remediation and rehabilitation
- **Concrete cosmetic repairs** — finishes, surface defects, making good
- **Concrete construction** — and project delivery, from a working PM's seat
- **Formwork** — design, build, striking, re-use
- **Academic knowledge and industry guidelines** — standards read properly
  (see §6 for sourcing rules)
- **News, trends, and AI tips & tricks** — what is changing and how to use it,
  for people in the industry or anyone curious

The site is a **personal** platform — not a company site, not a marketing brochure.
It is the author's public brain: what he knows, what he thinks, what he's watching,
what the work actually looks like. The audience is **anyone who works in concrete or
is curious about it** — peers first, generalists welcome.

## 4. The sections

| Section | Holds | Example first pieces |
|---|---|---|
| **Knowledge** | Technical guides grounded in standards | Concrete curing; spalling repair (live) — formwork, waterproofing, cosmetic repairs (next) |
| **AI & Concrete** | Practical AI tips and tricks for people in the industry | AI for inspection photo logs; drafting QA checklists (coming next) |
| **Ideas** | Frameworks and lessons from running construction work | Five lessons from building a regional operation (live) |
| **Trends** | What is changing: low-carbon concrete, digital delivery, precast advances | (coming next) |
| **News** | Short briefings with working commentary, newest first | Hub launch; aging building stock repair demand (live) |
| **Stories** | Sanitized field stories — lessons are the point | Strengthening a river bridge (live) |

Every piece ends with **sources** (see §6) and every section carries a "coming next"
list so the site visibly grows.

## 5. The GEO playbook (why the site is built the way it is)

> **Applied as the access engine, not a page topic.** The playbook *runs* the site — the
> operating plan is [`GROWTH.md`](GROWTH.md) and tracking is [`VISIBILITY.md`](VISIBILITY.md).
> (An explainer article about GEO was published 2026-08-08, then archived the same day —
> it misread the brief.)

Source: the five-step GEO method (Silicon Valley Girl, "How to Rank #1 in AI", 2026-08)
— the same playbook that took a podcast brand from invisible to 5th of 11 tracked
brands in two months.

1. **Machine-readable site** — static HTML, no build step, full text on every page, no
   JS-gated content.
2. **Structured data** — Schema.org JSON-LD: Person + WebSite, Article, CollectionPage,
   FAQPage. *(Add LinkedIn `sameAs` — open TODO.)*
3. **`llms.txt` + `sitemap.xml` + `robots.txt`** — the plumbing AI crawlers look for.
4. **Query-optimized content** — every article answers a real question someone in the
   industry (or a curious outsider) actually asks; FAQs are first-class content.
5. **Monthly visibility check** — re-ask the 5 diagnosis queries in ChatGPT, Claude,
   Perplexity; log in `VISIBILITY.md`. Two months is the realistic horizon for first
   movement.

The diagnosis queries are **knowledge queries, not contractor-referral queries** — the
hub competes on what people want to *learn* about concrete, which is a much bigger and
less contested pool than "recommend a repair contractor in Hamilton" (that framing was
retired in v1.1). The competitive window: ~92% of marketers say they'll optimize for AI
search, ~40% are doing it, and construction is almost entirely absent. The people who
publish now are the names AI recommends later.

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
- **Personal experience is fine and welcome** (Brazil precast, field stories) — label
  it as experience, never let it read as a standard.

## 7. The identity cluster (GEO step 3, strengthened)

The goal is a consistent, machine-readable identity across surfaces:

- **Concreteness** (site + brand) — the hub
- **Geraldo Monte** — the person (Person schema, author of every piece)
- **Concrete knowledge across precast, repairs (structural and cosmetic), construction
  and formwork — NZ + Brazil experience** — the domain
- **Anyone who works in concrete, or is curious** — the audience
- **LinkedIn** — add `sameAs` + keep active (open TODO)
- **Google Business Profile** — considered for the identity markers (open TODO)

## 8. Building blocks already done

- Live static site with 5 sections, 6 published pieces (all verified 200)
- GEO plumbing: schema.org on every page, `llms.txt`, `sitemap.xml`, `robots.txt`
- README plan: content rules, knowledge sourcing & copyright policy, monthly
  visibility check, TODOs
- 6 reviewed source notes in Technical_Knowledge behind the first two articles
- **Design identity selected 2026-08-08: C — Spec Sheet** — full spec in
  [`DESIGN.md`](DESIGN.md); three rendered directions for comparison in
  [`mockups/concreteness-identity-directions.html`](mockups/concreteness-identity-directions.html)

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
- [ ] Add "AI & Concrete" as a sixth site section now, or fold the first AI pieces into
      Ideas until there's a month of content to justify a section?
- [ ] How prominent should the Brazil precast angle be? (Differentiator — but keep it
      honest: experience, not a course.)

## 11. Measures of success

- **GEO (2-month horizon):** Concreteness or Geraldo Monte appears in ≥1 of the 5
  monthly diagnosis **knowledge** queries in any major AI (per `VISIBILITY.md`).
- **Reach:** site visits; AI-assistant referrals appear in analytics.
- **Identity:** LinkedIn `sameAs` live; consistent name across surfaces.
- **Content:** one new article per section per month; sources on every piece.
