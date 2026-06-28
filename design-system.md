# Design System — Unified, Dark Build (Reference)

Merged from two sources: Axios (Digital Agency WordPress theme — structured web UI) and Nova/Astra Studio (Instagram moodboard — black-and-neon editorial brutalism). This build recolors the merged system to techgear's dark, single-green-accent palette. Same components, same structure — only the color layer changed.

## Brand Thesis

Editorial brutalist energy, applied to a real, structured web product, now fully dark. One black page, one green accent, two elevated surface tones for rhythm. Same display face and label texture as before — the system just lost its light-mode option.

## What Changed From the Previous Build

| Token | Was | Now | Note |
|---|---|---|---|
| `--black` | `#0A0A0A` | `#121212` | Page background — now the single base, not just the "dramatic" tone |
| `--cream` | `#F2EFE3` (light paper) | `#1B1B1B` (dark surface) | Repurposed: elevated card/panel tone, not a light section |
| `--sage` | `#E9EFDC` (light paper) | `#242424` (dark surface) | Repurposed: secondary elevated tone for alternation |
| `--gray-mid` | `#6B6B6B` | `#9A9A9A` | Lightened — muted text now needs to read on dark, not light |
| `--white` | `#FFFFFF` | `#FFFFFF` | Unchanged |
| `--volt` | `#5FD53A` | `#5FD53A` | Unchanged — already matched the target palette |
| `--magenta` | `#FF3DA6` | `#FF3DA6` | Unchanged, still unused/reserved |

## Color Tokens

| Token | Hex | Usage |
|---|---|---|
| `--black` | `#121212` | Page background, the darkest dramatic blocks (hero) |
| `--white` | `#FFFFFF` | Headings, body text — the default text color now |
| `--cream` | `#1B1B1B` | Elevated surface — cards, navbar, stat blocks |
| `--sage` | `#242424` | Secondary elevated surface — alternation only |
| `--volt` | `#5FD53A` | The single accent — highlights, ticker, CTAs, icons, emphasis |
| `--magenta` | `#FF3DA6` | Rare second accent — one element per page max, optional |
| `--gray-mid` | `#9A9A9A` | Muted/secondary text on dark surfaces |

Rule: volt is the only accent doing real work. Black is the floor, cream/sage are what sits one step above it. There is no light section left in this build — "light vs dark" is now expressed as "page vs elevated surface," not "light page vs dark hero."

## Typography

Unchanged. Archivo Black (display, two casing modes), Space Mono (`//` labels), Inter (body). Casing still signals "moment vs page": UPPERCASE for hero/social/statements, sentence case for page headings — that logic doesn't depend on light or dark, it survives the recolor untouched.

## Radius Rule — Two-Tier

Unchanged. Structure = sharp (0px). Interaction = pill (999px).

## Grid & Spacing

Unchanged. 8px base scale. Same two valid grids (square social tiles, 12-col web).

## Components — What Changed

Everything below kept its layout and behavior. Only the fill/text logic adjusted for an all-dark page:

- **Cards (service, stat, radius demo, navbar, swatch meta)** — background moved from white to `--cream`; text now inherits white by default instead of black.
- **Inverted service card** — this is the one real structural color decision. With no light surface left to invert into, "emphasis" now means **volt fill + black text**, not black fill + white text. Still exactly one inverted card per row.
- **Dividers and hairline borders** (section rules, swatch borders, card borders, the accent-mark rule, footer rule) — moved from solid black to `rgba(255,255,255,0.15–0.25)`, since black-on-black is invisible.
- **Outline button** — text/border moved from black to white, for the same reason.
- **Section accent mark** — the two-square mark flipped polarity: filled square is now white (was black), the "hollow" square now shows black (was cream) to match the new true page background.
- **Quote card, mark-block, mark-pill, ticker** — unaffected. These already had their own explicit black-on-volt treatment and didn't depend on the page's light/dark state.

## Photography

Unchanged. Near-monochrome, never full color. Black-and-white duotone for social tiles; black-and-white with a dark gradient overlay for hero sections.

## Voice

Unchanged. Short and declarative on statement contexts; slightly warmer on page contexts. Still active voice, no filler, no exclamation points.

## Do / Don't

- Do: use UPPERCASE + block highlight for moments; sentence case + pill highlight for pages.
- Do: keep structure sharp, interaction round — don't mix the two on the same element.
- Do: use cream/sage to create surface rhythm instead of introducing a new hue.
- Don't: use more than one volt-inverted card per service row.
- Don't: let magenta appear more than once per page/tile.
- Don't: use full-color photography anywhere in the system.
- Don't: use a solid black border or divider on the page background — it's invisible now. Use white-at-low-opacity instead.
