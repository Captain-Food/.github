# thecaptaincompany.com — Landing page brief

> Living source of truth for THE CAPTAIN COMPANY marketing site
> (repo `thecaptaincompany.github.io`). Owned by the product owner; drafted with
> "Neuro" (neuromarketing/conversion). Update this doc as decisions are made.

> **Brand name:** the display/brand name is **THE CAPTAIN COMPANY** (three words,
> all-caps wordmark). `TheCaptainCompany` is only the GitHub org handle inside URLs
> and repo paths — never the visible brand name in copy.

- **Status:** Round 1 locked · brand system locked · Round 2 resolved — **ready to build** (one gap: WhatsApp link).
- **Last updated:** 2026-07-23
- **Target site:** `thecaptaincompany.com` (repo `TheCaptainCompany/thecaptaincompany.github.io`)

---

## Legal / operating status (IMPORTANT — honesty in copy)

THE CAPTAIN COMPANY **does not exist as a company yet**. It is currently an **initiative of the
Caring Hope Foundation** (same setup as Captain.Food), running under the Foundation until it becomes
self-sustaining. **It is not a cooperative** — do not describe it as one, or use ESUS / SCIC /
social-and-solidarity-economy language for it. The only status to state is: a Caring Hope Foundation
initiative.

**Éditeur (from Captain.Food's mentions-légales — same entity):** Association **Caring Hope
Foundation**, loi 1901, déclarée à Tours, **RNA W372020229**; siège Tours (Centre-Val de Loire),
France; directeur de publication = le·la représentant·e légal·e. Host: GitHub Pages.

---

## The fleet (context)

THE CAPTAIN COMPANY (parent) builds a spec-driven software factory and the products on top of it:

| Repo | What it is | Public surface |
| --- | --- | --- |
| `captain-studio` | UI to administer the specs | internal for now → **coming soon** |
| `captain-engine` | Spec templates, codegen & framework ("how we build") | internal for now → **coming soon** |
| `captain-food` | The flagship platform (in progress) | `live.` / `restos.` / `riders.` / `{slug}.captain.food` |
| `captain-food.github.io` | Captain.Food marketing site | `join.captain.food` |
| `thecaptaincompany.github.io` | **This** — the company marketing site | `thecaptaincompany.com` |

---

## Round 1 — strategy (LOCKED)

| Decision | Choice |
| --- | --- |
| **Primary goal** | **Route to products** — umbrella brand hub: establish credibility, send each visitor to the right product/action. No single hard conversion. |
| **Audience (priority)** | ① Future crew / talent · ② Technical builders · ③ Investors / public sector. **Not** restaurateurs (that is `join.captain.food`). |
| **Narrative** | **Mission-led** — a Caring Hope Foundation initiative building open, spec-driven tools against extractive platforms. (Not a cooperative.) |
| **Language** | **Bilingual FR + EN** (toggle). |

**Implication:** hero + primary CTA speak to crew/builders; the mission frames the whole page;
Captain.Food is living **proof**, not the pitch; restaurateur conversion is delegated to `join.captain.food`.

---

## Brand system (LOCKED — from the brand guide)

Reference sheets in-repo:
[`assets/brand/brand-logo-lockup.jpg`](assets/brand/brand-logo-lockup.jpg) ·
[`assets/brand/brand-style-guide.jpg`](assets/brand/brand-style-guide.jpg)

**Palette** (the company's OWN identity — black + gold, **not** Captain.Food's navy):

| Token | Hex | Use |
| --- | --- | --- |
| Black | `#000000` | text, primary/dark surfaces, reversed logo bg |
| Warm Gold | `#D4AF37` | brand accent, primary buttons, highlights |
| White | `#FFFFFF` | light surfaces |
| Soft Off-White | `#F8F8F8` | light section backgrounds |

**Typography**
- Scale: H1 72px Bold · H2 40px SemiBold · H3 24px SemiBold · Body 16px Regular · Caption 12px Regular.
- ✅ **Fonts:** no Apparat licence → substitute a free geometric display face. **Space Grotesk** for
  display/headings + **Montserrat** for body/UI (both free, Google Fonts). The wordmark is rendered from
  the logo asset, not live text.

**Voice** — nautical-leadership tone. Brand-guide sample taglines & cards ("Premium Yacht Systems" etc.)
are generic placeholders → **tone reference only**, not content.

**Components:** primary (gold-filled) / secondary (outline) / tertiary (text) buttons w/ hover+focus;
form fields (default/focus/error/select/checkbox); cards (featured/dark/trust); **4px spacing base**
(4/8/16/24/32/48/64/96). **Icons:** nautical · bold · clean · geometric.

**Logo usage:** primary · mark · reversed-on-dark · gold · social avatar · favicon · app icon. Dark mode
first-class.
- ✅ Individual files not available → **crop usable raster assets from the brand sheets**: light lockup
  (header/light), reversed lockup (dark sections/footer), mark, favicon, app icon. Transparent SVG/PNG can
  swap in later with no markup change.

---

## Round 2 — details (RESOLVED)

### A. Design & build ✅
- Reuse `captain-food.github.io`'s static stack (vanilla HTML/CSS/JS, `partials.js` pattern, GitHub Pages),
  but apply THE CAPTAIN COMPANY's own black+gold palette + typography.
- One-page bilingual landing now; legal pages mirrored from Captain.Food. Dark mode first-class.
- **Structure:** hero (mission one-liner + primary CTA) → "how we build" → **product cards** (Food / engine / studio)
  → mission + Caring Hope Foundation backing → CTAs per audience → footer.

### B. Product routing cards ✅
- **Captain.Food** — the one real product (in progress) → links to `join.captain.food`.
  One-liner: "0% commission food ordering for local restaurants — pilot in Tours."
- **captain-engine** & **captain-studio** — **coming soon** (internal for now), teaser cards, **no external link**.
  - captain-engine: "The spec-driven engine we build on: one source of truth, everything generated."
  - captain-studio: "Author and administer the specs, visually."

### C. Mission statement ✅ (adopted unless edited)
- **EN:** "THE CAPTAIN COMPANY is a Caring Hope Foundation initiative building open, spec-driven software
  that gives independents back control from extractive platforms — starting with Captain.Food, 0%
  commission food ordering for local restaurants. Everything we make is open source and built to last."
- **FR:** "THE CAPTAIN COMPANY est une initiative de la Caring Hope Foundation qui construit des logiciels
  ouverts, pilotés par la spécification, rendant aux indépendants le contrôle repris par les plateformes
  extractives — à commencer par Captain.Food, la commande en ligne à 0 % de commission pour les
  restaurants locaux. Tout ce que nous faisons est open source et conçu pour durer."

### D. Contact channels ✅
- **Primary email:** `contact@thecaptaincompany.com` (all audiences).
- **Builders:** link the GitHub org `github.com/TheCaptainCompany` ("explore the code").
- **Personal:** a **WhatsApp** CTA — "connect with me on WhatsApp".
  - 🔴 **Need the WhatsApp link/number** (`wa.me/…`). Building with a clearly-marked placeholder until provided.
- No other company socials for now (Instagram/LinkedIn/etc. belong to Captain.Food).

### E. Footer & legal ✅ (same as Captain.Food)
- Éditeur = Association Caring Hope Foundation (see status section). Host = GitHub Pages. Contact = `contact@thecaptaincompany.com`.
- Mirror `mentions-legales` + `confidentialite` from `captain-food.github.io`, re-branded.
- Footer bottom: "© 2026 THE CAPTAIN COMPANY — a Caring Hope Foundation initiative."

### F. Domain & repo ✅
- Custom domain **`thecaptaincompany.com`** (bare). `CNAME` file = `thecaptaincompany.com`.
- Product owner configures DNS + **`www` → bare** redirect; enable "Enforce HTTPS" once DNS resolves.
- Repo: `TheCaptainCompany/thecaptaincompany.github.io`.

---

## Decisions log
- 2026-07-23 — Round 1 strategy locked (goal / audience / narrative / language).
- 2026-07-23 — Brand name = **THE CAPTAIN COMPANY** (display, all-caps wordmark); `TheCaptainCompany` = GitHub handle only.
- 2026-07-23 — Brand system locked from the brand guide (palette black+gold, type, components, dark mode, logo usage). Sheets saved to `docs/assets/brand/`.
- 2026-07-23 — Status: **Caring Hope Foundation initiative**, not yet incorporated; **not a cooperative** (removed all coop/ESUS/SCIC framing).
- 2026-07-23 — Round 2 resolved: products (Food live, engine/studio coming-soon); fonts (Space Grotesk + Montserrat, no Apparat); email `contact@thecaptaincompany.com` + GitHub + WhatsApp; legal = Caring Hope Foundation (RNA W372020229); domain `thecaptaincompany.com`. One gap: WhatsApp link.
