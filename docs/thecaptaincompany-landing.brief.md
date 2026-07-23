# thecaptaincompany.com — Landing page brief

> Living source of truth for THE CAPTAIN COMPANY marketing site
> (repo `thecaptaincompany.github.io`). Owned by the product owner; drafted with
> "Neuro" (neuromarketing/conversion). Update this doc as decisions are made.

> **Brand name:** the display/brand name is **THE CAPTAIN COMPANY** (three words,
> all-caps wordmark). `TheCaptainCompany` is only the GitHub org handle inside URLs
> and repo paths — never the visible brand name in copy.

- **Status:** discovery — Round 1 locked · brand system locked · remaining facts open
- **Last updated:** 2026-07-23
- **Target site:** `thecaptaincompany.com` (repo `TheCaptainCompany/thecaptaincompany.github.io`)

---

## Legal / operating status (IMPORTANT — honesty in copy)

THE CAPTAIN COMPANY **does not exist as a company yet**. It is currently an **initiative of the
Caring Hope Foundation** (the same setup as Captain.Food), running under the Foundation until it
becomes self-sustaining. The **cooperative / ESUS / SCIC** form is an **ambition ("cap")**, not a
current legal status — copy must not claim it as fact.

- Public framing: "a Caring Hope Foundation initiative" — a credible, transparent backing signal.
- 🔴 Need: Caring Hope Foundation legal name, link, and the exact line/logo they want in the footer.

---

## The fleet (context)

THE CAPTAIN COMPANY (parent) builds a spec-driven software factory and the products on top of it:

| Repo | What it is | Public surface |
| --- | --- | --- |
| `captain-studio` | UI to administer the specs | _TBD_ |
| `captain-engine` | Spec templates, codegen & framework ("how we build") | _TBD_ |
| `captain-food` | The flagship platform | `live.` / `restos.` / `riders.` / `{slug}.captain.food` |
| `captain-food.github.io` | Captain.Food marketing site | `join.captain.food` |
| `thecaptaincompany.github.io` | **This** — the company marketing site | `thecaptaincompany.com` |

---

## Round 1 — strategy (LOCKED)

| Decision | Choice |
| --- | --- |
| **Primary goal** | **Route to products** — umbrella brand hub: establish credibility, send each visitor to the right product/action. No single hard conversion. |
| **Audience (priority)** | ① Future crew / talent · ② Technical builders · ③ Investors / public sector. **Not** restaurateurs (that is `join.captain.food`). |
| **Narrative** | A **mission-led cooperative** (in ambition) — builds open, spec-driven tools against extractive platforms. |
| **Language** | **Bilingual FR + EN** (toggle). |

**Implication:** hero + primary CTA speak to crew/builders ("come build with us / see how we
build"); the mission frames the whole page; Captain.Food is presented as living **proof**, not as
the pitch; clear secondary paths for partners/funders; restaurateur conversion is delegated out to
`join.captain.food`.

---

## Brand system (LOCKED — from the brand guide)

Reference sheets saved in-repo:
[`assets/brand/brand-logo-lockup.jpg`](assets/brand/brand-logo-lockup.jpg) ·
[`assets/brand/brand-style-guide.jpg`](assets/brand/brand-style-guide.jpg)

**Palette** (this is the company's OWN identity — black + gold, **not** Captain.Food's navy):

| Token | Hex | Use |
| --- | --- | --- |
| Black | `#000000` | text, primary surfaces, reversed logo bg |
| Warm Gold | `#D4AF37` | brand accent, primary buttons, highlights |
| White | `#FFFFFF` | light surfaces |
| Soft Off-White | `#F8F8F8` | light section backgrounds |

**Typography**
- **Display / headings:** Apparat. **Body / UI:** Montserrat.
- Scale: H1 72px Bold · H2 40px SemiBold · H3 24px SemiBold · Body 16px Regular · Caption 12px Regular.
- 🔴 **Font licensing:** Apparat is a commercial font (Positype). For a public web build I need either a
  licensed webfont kit, or approval to substitute a close free geometric display face (candidates:
  Michroma / Chakra Petch / Saira / Oxanium) for headings. Montserrat is free (Google Fonts).

**Voice / tagline** — nautical-leadership tone. Brand-guide samples ("LEAD THE WAY. OWN THE HORIZON.",
"LEAD WITH PURPOSE. NAVIGATE THE FUTURE.", "Navigate with clarity. Lead with honor.") are **tone
references only** — they're generic; final copy will marry this voice to the real mission and the
crew/builder audience. Likewise the brand sheet's sample cards ("Premium Yacht Systems", "Smart
Navigation Suite") are **placeholder** — ignore for content.

**Components** (defined in the guide, to mirror in CSS): primary (gold-filled) / secondary (outline) /
tertiary (text) buttons with hover+focus; form fields (default/focus/error/select/checkbox); card
components (featured / dark / trust); spacing scale on a **4px base** (4/8/16/24/32/48/64/96).

**Icon direction:** nautical · bold · clean · geometric; consistent stroke weight, rounded corners.

**Logo usage:** primary (full colour) · mark only · horizontal lockup (light bg) · **reversed (dark
bg)** · gold (premium) · social avatar · favicon · app icon. Dark mode is a first-class case.
- 🔴 Need the **individual logo/icon files** (SVG or transparent PNG) — the reversed-on-dark, gold, mark,
  favicon and app-icon variants — extracted from the sheets, so the site (and dark mode) render cleanly.

---

## Round 2 — details

Legend: ✅ = resolved / proposed default · 🔴 = still need from product owner.

### A. Design & build
- ✅ **Stack:** reuse `captain-food.github.io`'s approach — vanilla HTML/CSS/JS, `partials.js` pattern,
  static GitHub Pages — but apply **THE CAPTAIN COMPANY's own** palette + typography above (not Captain.Food's navy).
- ✅ **Scope:** one-page bilingual landing now; minimal legal pages once entity facts exist.
- ✅ **Dark mode:** first-class (brand guide provides light/dark). Uses reversed logo on `#000000`.
- ✅ **Structure:** hero (mission one-liner + primary CTA) → "how we build" → **product cards** (Food / engine / studio) → mission / cooperative-in-ambition + Caring Hope Foundation backing → CTAs per audience → footer.

### B. Product routing cards (core of the umbrella hub)
For each of Captain.Food, captain-engine, captain-studio:
- 🔴 **Public status** — live / in development / private / coming soon?
- 🔴 **URL to link** — Captain.Food → `join.captain.food`; engine/studio → own site, GitHub repo, or nothing yet?
- ✅ **One-liner** — drafts to approve:
  - **Captain.Food** — "0% commission food ordering for local restaurants — live pilot in Tours." → `join.captain.food`
  - **captain-engine** — "The spec-driven engine we build on: one source of truth, everything generated."
  - **captain-studio** — "Author and administer the specs, visually."

### C. Mission statement (company-level)
🔴 Approve / edit — drafts updated for the Foundation status:
- **EN:** "THE CAPTAIN COMPANY is a Caring Hope Foundation initiative building open, spec-driven software
  that gives independents back control from extractive platforms — starting with Captain.Food, 0%
  commission food ordering for local restaurants. Everything is open source; the cap is to become a
  cooperative of the social & solidarity economy once it sustains itself."
- **FR:** "THE CAPTAIN COMPANY est une initiative de la Caring Hope Foundation qui construit des logiciels
  ouverts, pilotés par la spécification, rendant aux indépendants le contrôle repris par les plateformes
  extractives — à commencer par Captain.Food, la commande en ligne à 0 % de commission pour les
  restaurants locaux. Tout est open source ; le cap est de devenir une coopérative de l'économie sociale
  et solidaire une fois l'autonomie atteinte."

### D. Conversion actions / contact channels (🔴 real values — won't invent)
- **Crew/talent:** email (`hello@` / `jobs@thecaptaincompany.com`?) or page? any open roles?
- **Builders:** link GitHub org `github.com/TheCaptainCompany`? newsletter/waitlist for the engine?
- **Investors/public sector:** contact email? Open Collective / transparency link?
- **General:** primary contact email + socials (LinkedIn / X / Mastodon / …).

### E. Footer & legal identity (🔴)
- Caring Hope Foundation legal name + link + the footer attribution/logo they want.
- Name founder/team on the page, or stay collective?
- Open Collective / public-accounts link (radical transparency, per the Captain.Food ethos).

### F. Domain & repo (🔴)
- Confirm `thecaptaincompany.com` (+ `www`?). DNS configured, or just drop the `CNAME` file for you to point?
- Confirm repo is exactly `TheCaptainCompany/thecaptaincompany.github.io` and empty/new (I'll add it to the session when we build).

---

## Decisions log
- 2026-07-23 — Round 1 strategy locked (goal / audience / narrative / language).
- 2026-07-23 — Brand name = **THE CAPTAIN COMPANY** (display, all-caps wordmark); `TheCaptainCompany` = GitHub handle only.
- 2026-07-23 — Brand system locked from the brand guide (palette black+gold, Apparat+Montserrat, components, dark mode, logo usage). Sheets saved to `docs/assets/brand/`.
- 2026-07-23 — Status clarified: THE CAPTAIN COMPANY is a **Caring Hope Foundation initiative** (not yet incorporated); cooperative form is an ambition. Copy must reflect this.
