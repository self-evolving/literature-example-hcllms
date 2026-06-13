# Reflections and New Directions for Human-Centered Large Language Models

This repository hosts a Quartz + Sepo Markdown edition of arXiv:2605.06901,
[“Reflections and New Directions for Human-Centered Large Language Models”](https://arxiv.org/abs/2605.06901)
(Ziems, Zhao, Yang, et al., Stanford University). It was produced from the
`self-evolving/literature-template` baseline using the `paper-to-site` skill.

The paper itself is the site entry point (`/`), and its full text is split into
section pages for readable navigation, popovers, and backlinks.

Durable content lives in this repository:

- `content/index.md` — hosted paper note and site entry point, with abstract, chapter outline, and source links.
- `content/ziems2026reflections/` — the converted section tree (eight chapters) and subsection pages.
- `content/ziems2026reflections/figures/` — figures from the arXiv TeX source, lowercased for deployment safety.
- `content/papers/` — reference area for cited-paper notes.
- `bibliography.bib` — BibTeX imported from the arXiv source so Markdown `[@key]` citations render.

The conversion keeps figures near their LaTeX source locations. Markdown/HTML
does not float figures the way LaTeX does, so placement is source-order rather
than page-layout exact. LaTeX cross-references (`\ref{sec:...}`, `\ref{fig:...}`)
were rewritten into descriptive internal links.

## Local development

Use Node `22.x`:

```bash
npm ci
npm run install-plugins
npm run dev
```

Useful commands:

```bash
npm run check       # tsc + prettier
npm run check:site  # check, restore plugins, and build
npm run build       # writes the static site to public/
```

`npm run dev` serves the Quartz site locally. `npm run build` writes the static
site to `public/`.

## Vercel configuration

Import the repository into Vercel with:

- Framework preset: **Other**
- Install command: `npm ci`
- Build command: `npm run build`
- Output directory: `public`

These settings are also captured in `vercel.json`.

Recommended Vercel environment variable:

| Name       | Value                                                                                  |
| ---------- | -------------------------------------------------------------------------------------- |
| `SITE_URL` | Production domain without protocol, e.g. `hcllms-survey.example.com` or a Vercel host. |

## Sepo comments

Comments are enabled by default on a best-effort basis. The shipped GitHub
Actions workflows prepare the fixed `SEPO_COMMENTS_*`, `SEPO_PREVIEW_*`, and
`HYPOTHESIS_*` build environment before Quartz runs: they default
`SEPO_COMMENTS_REPO` to this repository, default `SEPO_COMMENTS_CATEGORY=General`,
set pull request preview identity, and resolve the public GraphQL IDs needed by
the Sepo/Giscus-compatible widget.

If Discussions are disabled or IDs cannot be resolved, the default build logs a
warning and ships without comments. Set `SEPO_COMMENTS_ENABLED=true` for strict
build failures or `SEPO_COMMENTS_ENABLED=false` to opt out. Local/non-Actions
builds should pin `SEPO_COMMENTS_REPO_ID` and `SEPO_COMMENTS_CATEGORY_ID`.

## Sepo controls

Sepo workflows can be paused without disabling GitHub Actions globally by setting
the repository variable `AGENT_ENABLED=false`. Remove the variable or set it to
`true` to allow packaged `agent-*.yml` jobs to run again.
