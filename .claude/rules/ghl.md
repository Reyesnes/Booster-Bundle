---
paths:
  - "ghl/**"
---

# Go High Level (GHL) Rules

- **Always use the `ghl-code-builder` skill** to generate or edit any HTML+CSS+JS destined for a GHL Code element (landing pages, bridge pages, advertorials, VSLs, squeeze pages, funnel steps). Do not hand-write this code directly, even for small tweaks — GHL's block editor has rendering quirks the skill accounts for.
- Before editing code the owner pastes in, save the original as `ghl/pages/<page-slug>/source.html` (or `.txt` for a snippet) so there's a diffable baseline before changes.
- Keep each page/funnel step in its own subfolder under `ghl/pages/`, with a short `notes.md` describing its purpose (funnel step, offer, tracking/pixels embedded).
- This folder is a working/reference copy only — GHL pages are not deployed from this repo. The live site lives inside the GHL account; hand back the final code block(s) for the owner to paste in.
