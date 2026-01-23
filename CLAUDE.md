# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Academic research group website built with Hugo static site generator using the Hugo Blox (Wowchemy) theme. Content is managed via Markdown files with YAML frontmatter, optionally edited through Decap CMS.

## Development Commands

```bash
# Start local development server (http://localhost:1313/)
hugo server

# Start Decap CMS local backend (run in separate terminal)
npx decap-server

# Build for production
hugo --gc --minify
```

## Architecture

### Content Structure

All content lives in `content/` as Markdown with YAML frontmatter:
- **Team members**: `content/authors/{Name}/_index.md` with `avatar.jpg`
- **Publications**: `content/publication/{slug}/index.md` with optional `cite.bib`
- **Blog posts**: `content/post/{slug}/index.md`
- **Events**: `content/event/{slug}/index.md`
- **Homepage**: `content/_index.md`

### Configuration

Site config in `config/_default/`:
- `hugo.yaml` - Core Hugo settings
- `params.yaml` - Site parameters, theme, SEO, features
- `menus.yaml` - Navigation structure
- `module.yaml` - Hugo module imports (Bootstrap v5, Netlify plugin)

### CMS Configuration

Decap CMS config at `static/admin/config.yml` defines editable collections. Access CMS at `/admin/` when running both `hugo server` and `npx decap-server`.

### Automated Workflows

- **GitHub Pages deploy** (`.github/workflows/publish.yaml`): Triggers on push to main
- **Publications import** (`.github/workflows/import-publications.yml`): Converts `publications.bib` to Markdown via `academic` Python package, creates PR automatically

### Dependencies

- Hugo extended version 0.135.0
- Node.js (for Decap CMS local backend)
- Hugo modules: `blox-bootstrap/v5`, `blox-plugin-netlify`, `blox-plugin-decap-cms`
