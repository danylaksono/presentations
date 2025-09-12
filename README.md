This is a repository I use to store RevealJS and other HTML5 presentations.

## Quarto project

This repo is now a Quarto website for managing and publishing slide decks. Quarto supports `revealjs` slides and more; see the docs: `https://quarto.org/docs/presentations/`.

### Structure
- `_quarto.yml`: Project configuration and navbar
- `index.qmd`: Home page with a listing of decks
- `presentations/`: Place your `.qmd` slide decks here
  - `_metadata.yml`: Defaults for all decks (Revealjs theme/options)
  - `example.qmd`: Starter deck you can copy

### Create a new deck
1. Copy `presentations/example.qmd` to a new file, e.g., `presentations/my-talk.qmd`.
2. Edit the YAML title/author/date and slide contents.

### Preview and render
Install Quarto if needed (see `https://quarto.org/docs/get-started/`). Then, from the repo root:

```bash
quarto preview
```

To build the site to `_site/`:

```bash
quarto render
```

### Notes
- Deck defaults (theme, slide numbers, etc.) are set in `presentations/_metadata.yml` and apply to all decks in that folder.
