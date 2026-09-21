---
paths:
  - "docs/**/*.html"
---

# Legal Hub Rules (docs/)

- English is the default language and lives at the site root (`/`, `/privacy`, `/terms`, `/data-protection`, `/cookies`, `/data-deletion`). Spanish lives under `/es/` with the same path structure. `/en/` also exists as an explicit-English mirror of the root.
- **Every page must carry a language toggle** (the `.lang-toggle` block used across existing pages) linking EN ↔ ES, with the active language marked `class="active"`. Never ship a page without it.
- Any content change on an EN page must be mirrored on its ES counterpart, and vice versa. Keep both languages in parity — never leave one stale.
- Match the existing dark editorial brutalist styling exactly (see `design-system.md`): `--black:#121212`, `--volt:#5FD53A`, Archivo Black / Space Mono / Inter. Don't introduce new colors, fonts, or spacing tokens.
- Keep the responsable del tratamiento block (Nestor Reyes, NIE Z2377517N, Calle Bravo Murillo 91, Madrid) and `legal@boosterbundle.digital` consistent across every legal document.
- `/data-deletion` is a Meta/Facebook Developers requirement — never remove it, and keep its three deletion methods (email, form, panel) and the 30-day response / 6-year tax-record-retention language intact.
- This site deploys via GitHub Pages from `main` → `/docs`. `docs/CNAME` must keep pointing to `legal.boosterbundle.digital`.
