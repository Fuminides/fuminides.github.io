# Repository Guidelines

## Project Structure & Module Organization

This repository is a Jekyll 4 academic website based on the al-folio theme. Main site settings live in `_config.yml`. Page content is in `_pages/`, posts in `_posts/`, news items in `_news/`, projects in `_projects/`, and publications in `_bibliography/papers.bib`. Reusable Liquid templates are in `_includes/`, layouts in `_layouts/`, custom plugins in `_plugins/`, and SCSS in `_sass/`. Static assets are under `assets/`, especially `assets/img/`, `assets/pdf/`, `assets/js/`, and `assets/css/`. Structured CV and site data live in `_data/`.

## Build, Test, and Development Commands

- `bundle install`: install Ruby/Jekyll dependencies from `Gemfile`.
- `bundle exec jekyll serve --livereload`: run the site locally, usually at `http://localhost:4000`.
- `docker-compose up`: run the prebuilt al-folio container, exposed on port `8080`.
- `bundle exec jekyll build`: build the static site into `_site/`.
- `bundle exec jekyll build --lsi`: production-style build used by `bin/cibuild` and deployment.
- `npm install`: install Prettier and the Liquid plugin.
- `npx prettier . --check`: check formatting across Markdown, Liquid, YAML, JS, CSS, and SCSS files.

## Coding Style & Naming Conventions

Use two-space indentation in YAML, Markdown frontmatter, Liquid, and SCSS unless the surrounding file uses another style. Keep Liquid includes small and reusable. Follow existing frontmatter patterns for pages and collection items. Name news files `announcement_N.md`, projects `N_project.md`, and posts `YYYY-MM-DD-title.md`. Keep bibliography entries in valid BibTeX format and avoid hand-editing generated assets.

## Testing Guidelines

There is no dedicated unit test suite. Treat a successful Jekyll build as the primary validation. Run `npx prettier . --check` before opening a PR. For content-heavy changes, preview locally and check navigation, publication rendering, images, and external links. CI also runs Lychee broken-link checks on Markdown and HTML.

## Commit & Pull Request Guidelines

Recent history uses short imperative or descriptive commits such as `Update papers.bib` and `Fix`. Keep commits focused by content area. PRs should describe the visible site change, list validation commands run, link related issues when applicable, and include screenshots for layout, styling, or image changes.

## Agent-Specific Instructions

Before changing repository guidance, check both `AGENTS.md` and `CLAUDE.md` for overlapping instructions. Do not overwrite existing user edits in this dirty working tree; keep changes scoped to the requested files.
