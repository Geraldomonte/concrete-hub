# Concreteness — Design System & Identity Spec

> **Identity direction:** C — Spec Sheet (selected 2026-08-08 by owner ruling)
> **Comparison evidence:** [`mockups/concreteness-identity-directions.html`](mockups/concreteness-identity-directions.html)
> (A — Cast Slab and B — Field Journal remain comparison evidence only, not implementation alternatives.)
> **Status:** design-gate passed — ready for bounded build
> **Spec of record:** this file. The single token source is the `:root` block in `styles.css`.

---

## 1. Identity

**Character:** precise, technical, information-dense — engineering authority. The site reads
like a well-kept spec sheet: hairline rules, numbered mono metadata, sharp corners, and a
restrained spec-red annotation used only where a decision or caution needs to stand out.

**Why it fits Concreteness:** the brand promise is *"Concrete knowledge, made concrete"* —
specific, tangible, real. Spec-sheet precision is the visual form of that promise: no
decoration without function, every element justified, the standard separated from the
interpretation. It also matches the audience (construction people read specs every day) and
stays distinct from corporate construction marketing.

**Wordmark rule:** `CONCRETENESS` — uppercase, system sans bold, letterspaced `.06em`, no
logo mark. The tagline *"Concrete knowledge, made concrete."* sits under it in mono
uppercase small. No icon, no glyph — the typographic lockup IS the brand.

**Motion intent:** near-zero. Transitions are 150ms colour/border fades on interactive
elements only; no animation, no parallax, no scroll effects. Reduced-motion disables all.

## 2. Foundations — semantic tokens

Declared once in `:root` in `styles.css`. Components reference the **semantic** name, never
a raw hex. All text pairs verified WCAG AA (measured 2026-08-08).

### 2.1 Colour

| Token | Value | Role | AA on canvas | AA on surface |
|---|---|---|---|---|
| `--canvas` | `#eef0f2` | cool grey-white page background | — | — |
| `--surface` | `#ffffff` | raised panel / card / article surface | — | — |
| `--ink` | `#1f252b` | primary text | 13.5:1 | 15.5:1 |
| `--muted` | `#5b646d` | secondary/caption text | 5.3:1 | 6.0:1 |
| `--line` | `#d7dce1` | hairline borders / dividers | — | — |
| `--accent` | `#c23a17` | spec-red — links, annotations, current-state | 4.7:1 | 5.4:1 |
| `--accent-strong` | `#a02f10` | deeper spec-red — kickers, labels, emphasis | 6.3:1 | 7.2:1 |
| `--focus` | `#1769ff` | focus ring (≥3:1 against canvas/surface: 4.1:1 / 4.7:1) | — | — |

Rules: `--accent` is for links and small annotations; `--accent-strong` for uppercase
kickers and emphasis labels. Spec-red is never a large fill, never a background block.

### 2.2 Type

System stacks only — no web fonts, no CDN (per `self-improving-kb/conventions/frontend.md`
rule 1; keeps pages fast and fully crawlable for GEO).

| Role | Stack | Notes |
|---|---|---|
| Display / headings | `-apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, Arial, sans-serif` | bold, tight tracking |
| Body | same system sans stack | 16–17px, line-height 1.65 |
| Mono (metadata) | `ui-monospace, Menlo, Consolas, monospace` | kickers, labels, meta lines, table headers |

Scale: display `clamp(24px, 4vw, 32px)` / H2 `22px` / H3 `17px` / body `16px` / small
`14px` / eyebrow `12px` uppercase `.14em`. Kickers and section labels are mono uppercase.

### 2.3 Spacing, radius, elevation, breakpoints

- Spacing scale: `4 / 8 / 12 / 16 / 24 / 32 / 48 px`.
- Radius: `0` (sharp corners — the spec-sheet character). Interactive elements may use
  `2px` max where a corner needs softening; nothing rounded beyond that.
- Elevation: `0 1px 2px rgba(31,37,43,.06)` — a single hairline-shadow, no other elevation.
  Cards and articles rely on border + surface contrast, not shadows.
- Breakpoints: `900px` content max-width; grid collapse at `640px`; no horizontal body
  scroll at `390px`.

## 3. Components

Full interaction states per `conventions/frontend.md` rule 5: **default, hover,
focus-visible, active, disabled, loading** (loading N/A — static site, synchronous reads).

| # | Component | Anatomy | States & a11y |
|---|---|---|---|
| 1 | **Header / nav** | white surface, 2px hairline bottom rule in `--accent-strong`; wordmark lockup; horizontal nav with `aria-current` | current item: accent underline; hover: underline; focus-visible: ring; full keyboard order |
| 2 | **Kicker / eyebrow** | mono uppercase 12px `.14em`, `--accent-strong` | static |
| 3 | **Hero** | kicker + H1 + lede (`--muted`, max-width 60ch) | static |
| 4 | **Section card** | white surface, 1px hairline border, corner ticks (10px L-shaped `--accent-strong` marks, 55% opacity) | hover: accent border + 2px lift; focus-visible: ring; whole card is one focusable link |
| 5 | **Article prose** | white surface, hairline border, `padding 1.8rem 2rem` | static; headings mono/sans per scale |
| 6 | **Standard-says callout** | canvas background, 2px left rule in `--accent`, mono label "STANDARD SAYS" in `--accent-strong` | static; text always present (colour is reinforcement) |
| 7 | **In-practice callout** | canvas background, 2px left rule in `--muted`, mono label "IN PRACTICE" | static |
| 8 | **Field-note callout** | transparent, 1px dashed border `--accent` with 3px left rule, italic body, mono label "FIELD NOTE" | static; visually distinct from the two standard-grounded callouts |
| 9 | **Table** | full-width, hairline row borders, 2px `--ink` header rule, mono uppercase header row | wraps in `overflow-x:auto` container at 390px (no body scroll) |
| 10 | **FAQ** | `<details>` on canvas background, hairline border, bold summary | keyboard operable natively; focus-visible ring |
| 11 | **Standards & references block** | canvas background, hairline border, mono uppercase heading "STANDARDS AND REFERENCES" in `--accent-strong`, italic "own words" note, source list | static; every article carries one |
| 12 | **Footer** | hairline top border, `--muted`, about-line + disclaimer | static |

## 4. Patterns

| Pattern | Composition | Serves |
|---|---|---|
| **Standard vs interpretation** | callouts 6–8 on every knowledge article: what the standard says (paraphrased, linked) / what it means in practice / where personal field experience begins | Content rule: separate the standard from the interpretation |
| **Cited article anatomy** | article = intro → standard/practice/field-note callouts → body → table where useful → FAQ → Standards & references block | Copyright + sourcing rules (CONCEPT.md §6); GEO query coverage |
| **Honest absence** | "Coming next" lists on section pages; never a blank or placeholder task | Growth visibility; honest states rule |
| **Sanitized story framing** | Stories written generically ("a 1960s bridge over a braided river"); no client names, sites, values | Public-site content rule |
| **Machine-readable shell** | semantic HTML, full text in every page, schema.org JSON-LD (Person/WebSite, Article, CollectionPage, FAQPage), `llms.txt` + `sitemap.xml` + `robots.txt` in sync | GEO access engine (GROWTH.md) |

## 5. Governance

- **Single token source:** the `:root` block in `styles.css`. This DESIGN.md is the spec of
  record; no value is restated in component code.
- **Change rule:** any token/component/pattern change is an edit to this spec **before**
  code. No new component without a DESIGN.md entry (§3 table).
- **Identity lock:** A and B directions are closed. Re-opening a direction needs a new
  owner ruling, not a CSS tweak.
- **Version:** v1 bounded build (2026-08-08). Expansion — new component, sixth section,
  custom domain rebrand — is a separate owner decision recorded here.

## 6. Validation gates (run at build, re-run on any change)

- [ ] WCAG AA contrast on every text pair (measured values in §2.1 — re-verify any new pair ≥4.5:1, focus ≥3:1)
- [ ] Full keyboard traversal; visible `--focus` ring; no keyboard trap; focus returns after any disclosure toggle
- [ ] `prefers-reduced-motion: reduce` disables all transitions
- [ ] No horizontal body scroll at 390px; tables scroll in their own container
- [ ] Zero console errors; zero external network requests (offline, system fonts only)
- [ ] GEO sync: every new page updates `llms.txt` + `sitemap.xml`; schema.org JSON-LD per page type; full article text present in HTML

## 7. Open items (owner decisions, not gate failures)

- [ ] **AI & Concrete as a 6th nav section** — nav is flex-wrap, so adding it is a one-line
      change; decide when there's a month of content to justify it (CONCEPT.md §10)
- [ ] **Subtitle treatment** — CONCEPT.md asks full "Concreteness" vs keeping a subtitle;
      the lockup spec (§1) uses full "Concreteness" + tagline; confirm
- [ ] **Custom domain rebrand** — when `concreteness.co.nz` DNS lands, canonical URLs and
      schema `WebSite`/`Person` `@id` move to the custom domain; token system unaffected
- [ ] **LinkedIn `sameAs`** — add to Person schema once the URL is provided (GROWTH.md §4)
