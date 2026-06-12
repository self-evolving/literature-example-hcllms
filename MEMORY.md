# Durable Memory

## Durable

- Content for each imported paper lives under `content/<citationkey>/` with numbered chapter subdirs, `_meta.json` nav files, and a `figures/` dir; `content/papers/` holds reference notes only.
- Quartz config pattern for paper sites: remove `folder.positions.right: []` from `quartz.config.yaml` so section index pages show the graph; relax `library-page`/`not-index` conditions in `quartz.ts` so root and section pages render with full chrome (sidebar, header, backlinks).
- `quartz/styles/custom.scss` should have landing-page-specific CSS stripped when converting a template to a single-paper site (the `body[data-slug="index"]` block was removed in PR #2).
- The `/answer` skill is active on this repo — users tag `@sepo-agent /answer <question>` in giscus discussions on paper pages to request summaries.
- `bibliography.bib` in the repo root holds the full paper bibliography (~22k lines for 2605.06901); it is imported alongside content, not generated.
- Comments use sepo.js drawer: `Comments.tsx` emits a `sepo-embed` config div; sepo.js loads from `GISCUS_APP_HOST` (default `https://comment-api.sepo.sh`); drawer UI ships from comment service.
