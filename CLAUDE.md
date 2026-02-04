# CLAUDE.md - Project Guide

## Overview

Academic personal website for **Javier Fumanal Idocin** (Postdoc YUFE MSCA fellow at University of Essex). Built with **Jekyll** using the **al-folio** theme. Deployed automatically to GitHub Pages at `https://fuminides.github.io/`.

## Tech Stack

- **Jekyll 4.x** (Ruby-based static site generator)
- **al-folio theme** - academic-focused theme
- **Bootstrap 4 + MDB** - CSS framework
- **jekyll-scholar** - BibTeX bibliography management
- **SCSS** for styling
- **GitHub Actions** for CI/CD

## Key Files & Directories

| Path | Purpose |
|------|---------|
| `_config.yml` | Main site configuration (metadata, plugins, scholar settings) |
| `_pages/about.md` | Landing page / homepage |
| `_pages/research.md` | Research interests overview (rule-based learning, XAI, uncertainty, fuzzy) |
| `_pages/publications.md` | Publications page (auto-generated from BibTeX) |
| `_pages/projects.md` | Project showcase |
| `_pages/exfuzzy.md` | Dedicated page for Ex-Fuzzy library |
| `_pages/cv.md` | Curriculum vitae |
| `_bibliography/papers.bib` | BibTeX file with all publications |
| `_data/cv.yml` | Structured CV data |
| `_news/` | News/announcements (markdown files) |
| `_projects/` | Project showcase pages |
| `_sass/` | SCSS stylesheets |
| `assets/img/` | Images (responsive variants: 480px, 800px, 1400px) |
| `_includes/` | Reusable Liquid template partials |
| `_layouts/` | Page templates |

## Navigation Order

Pages appear in navbar based on `nav_order` in frontmatter:
1. Research (`nav_order: 1`)
2. Publications (`nav_order: 2`)
3. Projects (`nav_order: 3`)
4. Ex-Fuzzy (`nav_order: 4`)
5. CV (`nav_order: 5`)

## Common Tasks

### Add a new publication
1. Edit `_bibliography/papers.bib` - add BibTeX entry
2. Publications page auto-generates from this file

### Add news/announcement
1. Create file in `_news/` (e.g., `_news/announcement_X.md`)
2. Use frontmatter: `layout: post`, `date: YYYY-MM-DD`, `inline: true`

### Add a project
1. Create file in `_projects/` (e.g., `_projects/X_project.md`)
2. Include frontmatter with `title`, `description`, `img`, `importance`

### Update CV
Edit `_data/cv.yml` for structured data, or `_pages/cv.md` for layout changes

### Modify styling
- Global styles: `_sass/_base.scss`
- Theme variables: `_sass/_themes.scss`
- Component-specific: `_sass/_*.scss` files

## Local Development

```bash
# With Docker (recommended)
docker-compose up

# Or with Ruby/Bundler
bundle install
bundle exec jekyll serve --livereload
```

Site runs at `http://localhost:4000` (or port 8080 with Docker)

## Build Commands

```bash
# Standard build
bundle exec jekyll build

# Build with LSI (used in deployment)
bundle exec jekyll build --lsi
```

## Configuration Notes

- **Author name**: "Javier Fumanal Idocin" (used in jekyll-scholar)
- **Citation style**: APA
- **Dark mode**: Enabled
- **Math support**: MathJax enabled
- **Social links**: GitHub, Google Scholar, ORCID configured in `_config.yml`

## Deployment

Automatic via GitHub Actions:
1. Push to `master` branch
2. `broken-links.yml` workflow runs first
3. `deploy.yml` builds and deploys to GitHub Pages

## File Naming Conventions

- News: `announcement_N.md` (N = sequential number)
- Projects: `N_project.md` (N = display order/importance)
- Posts: `YYYY-MM-DD-title.md`
