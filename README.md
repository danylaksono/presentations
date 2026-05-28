This is a repository I use to store RevealJS and other HTML5 presentations.

## Quarto project

This repo is now a Quarto website for managing and publishing slide decks. Quarto supports `revealjs` slides and more; see the docs: `https://quarto.org/docs/presentations/`.

### Structure
- `_quarto.yml`: Project configuration and navbar
- `index.qmd`: Home page with a listing of top-level deck folders
- `cgvc2025/`: A published deck. Its URL is `/presentations/cgvc2025/`.
- `_templates/revealjs-deck/`: Starter folder to copy for a new deck
- `_archive/`: Older experiments and single-file examples that should not be rendered

### Create a new deck
1. Copy the template folder, e.g. `cp -R _templates/revealjs-deck cgvc2026`.
2. Edit `cgvc2026/index.qmd`.
3. Put images, GIFs, and other media in `cgvc2026/assets/`.

This produces a deck at `/presentations/cgvc2026/` once the site is rendered and published.

### Preview and render
Install Quarto if needed (see `https://quarto.org/docs/get-started/`). Then, from the repo root:

```bash
quarto preview
```

To build the site to `docs/`:

```bash
quarto render
```

### Notes
- The home page lists top-level `*/index.qmd` decks.
- Keep complete talks in their own top-level folders so each talk can carry its own assets and CSS.
- Older single-file deck examples were moved to `_archive/single-file-decks/`.
