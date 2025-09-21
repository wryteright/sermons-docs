# Hugo Book — Sermons (Bilingual: English + Telugu)

- Tile-based landing page (per language) linking to docs sections.
- Safe links using Hugo `relref` so URLs work whether this site is standalone or linked from another homepage.
- External homepage menu item (replace URL in `config.yml`).

## Local dev

1) Install Hugo (Extended).
2) Fetch theme as submodule:
   ```bash
   git init
   git submodule add https://github.com/alex-shpak/hugo-book themes/hugo-book
   ```
3) Run:
   ```bash
   hugo server -D
   ```

## Deploy (GitHub Pages)
- Push to `main`. Workflow builds & deploys.
- GitHub → Settings → Pages → Source: GitHub Actions.

## Content locations
- English: `content/en/docs/...`
- Telugu:  `content/te/docs/...`
- Homepage per language: `content/en/_index.md`, `content/te/_index.md`

Replace the external homepage URL in `config.yml` when integrating with your main site.