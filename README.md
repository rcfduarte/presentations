# Presentations

Monorepo of Slidev presentation decks by Renato Duarte.

Each subdirectory `<YYYY-MM>-<slug>/` is a complete Slidev project. The `theme/` symlink points to the canonical CNC-Editorial theme (in the Obsidian vault at `~/Desktop/Assets/slidev-themes/cnc-editorial/`).

## Build

```bash
cd <deck-slug>
pnpm install
pnpm dev       # local preview on http://localhost:3030
pnpm build     # static HTML build in dist/
pnpm export    # PDF export
pnpm validate  # check figure manifest
```

## Deploy

Push to `main` → GitHub Action builds + deploys to `gh-pages` → live at `https://rcfduarte.github.io/presentations/<slug>/`.

## New deck

```bash
cp -r _template/ 2026-05-my-new-talk/
cd 2026-05-my-new-talk
# edit slides.md, add figures to public/figures/, update _manifest.yaml
```

Or invoke via Claude: `claude "Start a research talk on <topic>"`.
