# Booster Bundle

Booster Bundle is a digital infoproducts / PLR / community business run by Nestor Reyes. This repository is the **operations base**: the public legal hub, the working copy of the Go High Level (GHL) marketing site, and the content/ads/growth strategy workspace.

## Repository Map

- `docs/` — **Legal Hub**, deployed via GitHub Pages to `legal.boosterbundle.digital`. Bilingual: EN default at `/`, ES at `/es/`, explicit EN mirror at `/en/`. Read `.claude/rules/legal-hub.md` before editing anything here.
- `ghl/` — Working snapshots of the main marketing site, which is actually built and hosted **inside Go High Level (GHL)**, not in this repo. Read `.claude/rules/ghl.md` first — **always use the `ghl-code-builder` skill** for any GHL page code.
- `content/` — Content and ads creation: calendars, ad copy, social content, brand voice reference.
- `strategy/` — Scaling strategy: roadmap, OKRs, positioning/market notes.
- `design-system.md` / `design-system.html` — Dark editorial brutalist design system shared across the Legal Hub and, where applicable, GHL pages.

## Git Workflow

- **Work only on `main`.** Do not create feature branches for this project — standing instruction from the owner. Commit directly to `main` and push with `git push -u origin main`.

## Legal / Compliance Reference

Use these exact details in any legal, privacy, or compliance content:

- Responsable del tratamiento: **Nestor Reyes** (NIE: Z2377517N)
- Dirección: Calle Bravo Murillo, 91, 28003 Madrid, España
- Contacto legal: legal@boosterbundle.digital
- Frameworks: RGPD (EU 2016/679), LOPD-GDD (España), LSSI-CE, Meta/Facebook Developers data-deletion requirements.

## Go High Level (GHL) — Main Website

The main Booster Bundle website is built inside GHL's funnel/website Code-element editor, not as a standalone codebase. The owner will paste in the current embedded HTML/CSS/JS for review or changes.

**IMPORTANT: always invoke the `ghl-code-builder` skill before writing or editing any GHL page/funnel code.** It produces production-ready, GHL-safe HTML+CSS+JS blocks for that editor. Never hand-write GHL code without it, even for a small tweak.

When the owner pastes GHL code, save a snapshot under `ghl/pages/<page-slug>/source.html` before editing, so changes stay diffable.

## Design System

Dark editorial brutalist. Base black `#121212`, single accent volt `#5FD53A`. Archivo Black (display), Space Mono (labels), Inter (body). Sharp corners for structure, pill radius for interactive elements. Full reference: `design-system.md`.

## Working with Claude Code Here

- This project spans distinct workstreams (legal hub, GHL site, content/ads, strategy). Run `/clear` when switching between them so context stays relevant.
- Specialized subagents live in `.claude/agents/`: `legal-hub-editor`, `ghl-maintainer`, `content-strategist`. Delegate to them explicitly, or let Claude pick based on the task description.
- Each subagent keeps its own project memory under `.claude/agent-memory/<name>/` (git-tracked) — it checks this before starting and updates it when done, so decisions and conventions persist across sessions.
