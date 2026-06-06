# Project: literature-example-hcllms

## Goals

Demonstrate the `self-evolving/literature-template` Quartz site pattern by hosting a real arXiv paper as a browsable, interlinked literature site. Serves as a reference example for the template.

## Current paper

- **arXiv 2605.06901** — "Reflections and New Directions for Human-Centered Large Language Models" (Ziems, Zhao, Yang et al., Stanford, 2026)
- Imported via the `paper-to-site` skill (PR #2, merged 2026-06-05)
- Content under `content/ziems2026reflections/` — 8 chapters, ~34 pages

## Site

- URL: `hcllms.sepo-preview.xyz`
- Build: `npm run build` → `public/` (Vercel: framework Other, install `npm ci`, build `npm run build`, output `public`)

## Constraints

- Quartz-based static site; no server-side logic
- Paper content is the single primary example; `content/papers/` holds reference notes only
- `content/notes/` (template demo notes) was removed when the paper was imported

## Open Questions

- PRs #1 (dependabot CI action bumps), #3 (npm prod deps bump), #5 (Giscus sepo-host), and #6 (responsive sidebar) are open — all need review/merge.
- The `/answer` workflow IS wired up — discussion #4 was answered by sepo-agent-app within ~4 min on 2026-06-05.
