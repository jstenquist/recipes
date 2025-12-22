# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Jekyll-based recipe blog deployed to GitHub Pages at recipes.stenquist.com. Uses minima theme.

## Commands

```bash
# install deps
bundle install

# local dev server (auto-reloads on changes, except _config.yml)
bundle exec jekyll serve

# build site
bundle exec jekyll build
```

## Adding Recipes

Create markdown file in `_posts/` with format: `YYYY-MM-DD-recipe-name.markdown`

Front matter:
```yaml
---
layout: post
title:  "Recipe Title"
date:   YYYY-MM-DD HH:MM:SS -0500
categories: dinner  # or breakfast, family, etc.
---
```

## Deployment

Auto-deploys via GitHub Actions on push to master. Workflow in `.github/workflows/jekyll-gh-pages.yml`.
