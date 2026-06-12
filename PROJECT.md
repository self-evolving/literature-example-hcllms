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

- PR #1 (dependabot CI action bumps) is open — needs review/merge. PR #3 (npm prod deps bump) was closed unmerged 2026-06-12.
- PR #8 (sepo.js drawer + deployment events template sync) merged 2026-06-12; closes issue #7.
- PR #5 (Giscus sepo-host) was closed 2026-06-11 — superseded by PR #8.
- PR #6 (responsive sidebar toolbar) was closed unmerged; responsive layout fix may resurface as future work.
- `agent/rubrics` branch has not been initialized — `/review` calls return N/A scoring. Run `Agent / Rubrics / Initialization` workflow to bootstrap.
- The `/answer` workflow IS wired up — discussion #4 was answered by sepo-agent-app within ~4 min on 2026-06-05.
