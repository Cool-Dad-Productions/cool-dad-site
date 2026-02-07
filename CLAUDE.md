# CLAUDE.md

This is a Jekyll-based personal portfolio site for cooldad.computer, showcasing whimsical coding projects.

## Quick Reference

```bash
# Local development
bundle exec jekyll serve

# Install dependencies
bundle install
```

Site runs at http://localhost:4000

## Project Structure

- `_posts/` - Project posts (format: `YYYY-MM-DD-title.md`)
- `_layouts/` - Page templates (page.html, post.html)
- `_includes/` - Reusable HTML partials
- `_sass/` - SCSS stylesheets
- `assets/main.scss` - Main stylesheet entry point
- `_config.yml` - Jekyll configuration
- `branding/style-guide.md` - Full brand guidelines

## Tech Stack

- Jekyll 4.2.2 with jekyll-theme-console
- Ruby with Bundler
- SCSS for styling
- GitHub Pages compatible
- RSS feed via jekyll-feed plugin (`/feed.xml`)

## Content Guidelines

- Write in first person, conversational tone
- Be technically specific but accessible
- Embrace honest reflections about challenges
- Avoid marketing speak and buzzwords

### Project Post Format

```yaml
---
layout: post
title: "Project Title"
tags: python, api, experiment
description: "Short description"
---
```

- Title: 3-8 words, descriptive but punchy
- Tags: 2-5 tags, lowercase (e.g., python, tool, learning-project)
- Description: 2-3 sentences, max 280 characters

## Skills

Custom Claude Code skills for this project:

- `/new-post` - Scaffold a new project blog post with proper frontmatter and structure. Prompts for title, tagline, description, and tags.

## Styling

Consult `branding/style-guide.md` for all style decisions including colors, typography, spacing, and components.

When making style changes:
1. Read the style guide first to understand existing patterns
2. Apply changes consistently with the documented system
3. Update the style guide to reflect any new patterns or modifications

When making CSS/styling changes, check all related components and files for consistency. Use Glob to find all files that might need updates (e.g., `*.scss`, `*.css`, `*.tsx` with className).
