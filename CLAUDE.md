# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Landing page for Simplelines (simplelines.co), a software company. Hosted on GitHub Pages using Jekyll with the `minima` theme.

## Development Commands

```bash
# Install dependencies
bundle install

# Run local development server (http://localhost:4000)
bundle exec jekyll serve

# Build site without serving
bundle exec jekyll build
```

## Prerequisites

- Ruby (>= 2.7)
- Bundler (`gem install bundler`)

## Architecture

- **Jekyll static site** deployed via GitHub Pages from the `master` branch
- `_config.yml` — site configuration (title, URL, theme)
- `index.md` — landing page content
- `Gemfile` — uses `github-pages` gem which pins Jekyll and plugins to match GitHub Pages environment
- Theme: `minima` (GitHub Pages default, provides layouts and styling)

## Deployment

Push to `master` branch. GitHub Pages builds and deploys automatically. Custom domain: simplelines.co (configured via DNS, not in this repo yet).
