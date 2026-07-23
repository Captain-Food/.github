# thecaptaincompany.com — Landing page brief

> Living source of truth for the TheCaptainCompany marketing site
> (repo `thecaptaincompany.github.io`). Owned by the product owner; drafted with
> "Neuro" (neuromarketing/conversion). Update this doc as decisions are made.

- **Status:** discovery — Round 1 locked, Round 2 open
- **Last updated:** 2026-07-23
- **Target site:** `thecaptaincompany.com` (repo `TheCaptainCompany/thecaptaincompany.github.io`)

---

## The fleet (context)

TheCaptainCompany (parent) builds a spec-driven software factory and the products on top of it:

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
| **Narrative** | A **mission-led cooperative** — builds open, spec-driven tools against extractive platforms. |
| **Language** | **Bilingual FR + EN** (toggle). |

**Implication:** hero + primary CTA speak to crew/builders ("come build with us / see how we
build"); the cooperative mission frames the whole page; Captain.Food is presented as living
**proof**, not as the pitch; clear secondary paths for partners/funders. Restaurateur conversion
is delegated out to `join.captain.food`.

---

## Round 2 — details (OPEN)

Legend: ✅ = proposed default, I'll proceed unless told otherwise · 🔴 = need from product owner (I won't invent facts).

### A. Design & build
- ✅ **Reuse** the `captain-food.github.io` stack & design system: vanilla HTML/CSS/JS, `styles.css`, `partials.js`, navy `#0e3a5f` + gold palette, same fonts — adapted with the TheCaptainCompany logo. Fast, consistent, on-brand.
- ✅ **Scope:** one-page landing now; add minimal legal pages (`mentions-legales`, `confidentialite`) only once the legal entity facts exist.
- 🔴 **Logo on dark mode:** current asset is a white-background JPEG (shows a white box on dark). A transparent PNG/SVG would fix it.

### B. Product routing cards (the core of an "umbrella hub")
For each of Captain.Food, captain-engine, captain-studio:
- 🔴 **Public status** — live / in development / private / coming soon?
- 🔴 **URL to link** — e.g. Captain.Food → `join.captain.food`; engine/studio → own site, GitHub repo, or nothing yet?
- ✅ **One-liner** — I'll draft, you approve. Working drafts:
  - **Captain.Food** — "0% commission food ordering for local restaurants — live pilot in Tours." → `join.captain.food`
  - **captain-engine** — "The spec-driven engine we build on: one source of truth, everything generated."
  - **captain-studio** — "Author and administer the specs, visually."

### C. Company mission statement (company-level, not product-level)
🔴 Approve / edit these drafts, and confirm the cooperative status:
- **EN (draft):** "TheCaptainCompany is a cooperative software company. We build open, spec-driven tools that give independents back control from extractive platforms — starting with Captain.Food, 0% commission food ordering for local restaurants. Everything we make is open source, built to last, and meant to become a digital commons."
- **FR (draft):** "TheCaptainCompany est une entreprise coopérative du logiciel. Nous construisons des outils ouverts, pilotés par la spécification, qui rendent aux indépendants le contrôle repris par les plateformes extractives — à commencer par Captain.Food, la commande en ligne à 0 % de commission pour les restaurants locaux. Tout ce que nous faisons est open source, durable, et destiné à devenir un bien commun numérique."
- 🔴 **Cooperative/ESUS/SCIC status:** already legally established, or still a *cap* (ambition)? Captain.Food materials phrase it as an ambition — I will not claim a legal status you don't hold.

### D. Conversion actions / contact channels (🔴 need real values — won't invent)
- **Crew/talent CTA:** email (e.g. `hello@` / `jobs@thecaptaincompany.com`?) or a page? Any open roles to list?
- **Builders CTA:** link to the GitHub org (`github.com/TheCaptainCompany`)? A newsletter/waitlist for the engine?
- **Investors/public-sector CTA:** contact email? Open Collective / transparency link?
- **General:** primary contact email + social links (LinkedIn / X / Mastodon / …).

### E. Company identity for footer & legal (🔴)
- Legal name of the entity, city (Tours?), any registration (SIREN), contact email.
- Name founder/team on the page, or stay collective?
- Open Collective / public-accounts link (radical transparency, per the Captain.Food ethos)?

### F. Domain & repo (🔴)
- Confirm custom domain `thecaptaincompany.com` (+ `www` redirect?). Is DNS configured, or should I just add the `CNAME` file and you point DNS?
- Confirm the repo is exactly `TheCaptainCompany/thecaptaincompany.github.io` and it's empty/new (I'll add it to the working session when we build).

---

## Decisions log
- 2026-07-23 — Round 1 strategy locked (see table above).
