# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Commands

```bash
# Local dev server (live reload, uses localhost:4000)
bundle exec jekyll serve --livereload

# Build only
bundle exec jekyll build

# Install dependencies
bundle install
```

## Architecture

This is a Jekyll academic personal website based on the [academicpages](https://github.com/academicpages/academicpages.github.io) template.

**Key content files:**
- `_pages/about.md` — homepage (bio, awards, research interests)
- `_pages/publications.md` — publication list, rendered via Liquid loops over `_data/publist.yml`
- `_pages/cv.md`, `_pages/talks.md`, `_pages/teaching.md`, `_pages/team.md`, `_pages/service.md`

**Publications** are managed entirely in `_data/publist.yml`. Each entry has: `title`, `authors`, `year` (integer), `link.url`, `link.display`, `highlight`. The `publications.md` page iterates over this file grouped by year — to add a paper, add an entry to `publist.yml`.

**Awards and honors** are in the `_pages/about.md` front matter as a Markdown list under `Selected Honors and Awards`. Entries follow the pattern:
```markdown
* **Award name** (Org - Year) [[link](url)]
```

**Navigation** is configured in `_data/navigation.yml`. Layout templates are in `_layouts/`, partials in `_includes/`.

The dev config `_config.dev.yml` overrides `url` to `http://localhost:4000` and disables analytics — use it with `--config _config.yml,_config.dev.yml` if needed (the default `jekyll serve` is sufficient for local dev).
