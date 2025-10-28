# Repository Guidelines

## Project Structure & Module Organization
- Root content pages: `about.md`, `contact.md`, `index.md`, `research.md`, etc.
- Configuration: `_config.yml` (primary), `_config_alfolio.yml` (alt theme).
- Assets: `assets/img/` for images referenced in Markdown.
- Dependencies: `Gemfile` (Jekyll, plugins). Generated output `_site/` is ignored.

## Build, Test, and Development Commands
- Install deps: `bundle install`
- Run locally with live reload: `bundle exec jekyll serve`
  - Visit `http://localhost:4000`
- Production build: `bundle exec jekyll build`
- Troubleshooting: `bundle exec jekyll serve --trace` and `bundle update`

## Coding Style & Naming Conventions
- Markdown: wrap at ~100 chars; use ATX headings (`#`, `##`).
- YAML/Config: 2‑space indentation; keep keys alphabetical where practical.
- Filenames: kebab-case (`publications.md`, `project-notes.md`).
- Images: place under `assets/img/`, reference relatively (e.g., `![Alt](assets/img/hero.png)`).
- Front matter: minimal, valid YAML. Example:
  ```yaml
  ---
  title: Research
  layout: page
  permalink: /research/
  ---
  ```

## Testing Guidelines
- Build check: `bundle exec jekyll build` finishes without errors/warnings.
- Local QA: click through nav, verify images, and validate external links.
- Content review: check spelling, headings hierarchy, and mobile layout.
- Optional (manual): run a link checker before PR if making many edits.

## Commit & Pull Request Guidelines
- Commits: imperative mood and scoped, e.g., `content: add antibody case study`, `config: enable sitemap`.
- Keep commits small and focused; reference issues with `#ID` when relevant.
- PRs must include:
  - Summary of changes and rationale.
  - Screenshots or GIFs for visual updates (desktop + mobile if UI changes).
  - Any config toggles touched (files, keys).

## Security & Configuration Tips
- Do not commit secrets or tokens; none are required for local builds.
- Avoid committing `_site/`, `.jekyll-cache/`, `vendor/` (already ignored).
- When changing themes/plugins, update both `Gemfile` and `_config*.yml` consistently.
