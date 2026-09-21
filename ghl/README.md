# GHL Working Copy

This folder holds **working snapshots** of the Booster Bundle main website, which is built and hosted inside Go High Level (GHL)'s funnel/website Code-element editor. Nothing here deploys automatically — it's a reference/diff base so changes to GHL-embedded code are trackable in git.

## Rules

- Always use the `ghl-code-builder` skill to generate or edit code for this site (see `.claude/rules/ghl.md`).
- One subfolder per page/funnel step under `pages/`, e.g. `pages/home/`, `pages/checkout-upsell/`.
- Each page folder: `source.html` (latest snapshot pasted from GHL) + `notes.md` (purpose, funnel step, tracking/pixels).

## Structure

```
ghl/
└── pages/
    └── <page-slug>/
        ├── source.html
        └── notes.md
```

Pages will be added here as the owner shares the current GHL-embedded code.
