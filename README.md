# cooldad.computer

A personal portfolio site for whimsical, purpose-built coding projects. Built with Jekyll using a customized console theme.

## Local Development

```bash
# Install dependencies
bundle install

# Run the development server
bundle exec jekyll serve
```

Open http://localhost:4000

## Project Structure

```
_posts/          # Project posts (YYYY-MM-DD-title.md)
_layouts/        # Page templates
_includes/       # Reusable HTML partials
_sass/           # SCSS stylesheets
assets/          # Main stylesheet and static assets
branding/        # Style guide and brand assets
```

## Adding a Project

Create a new file in `_posts/` with the format `YYYY-MM-DD-project-name.md`:

```yaml
---
layout: post
title: "Project Title"
tags: python, api, experiment
description: "Short description"
---

Project content here...
```

## Style Guide

See [branding/style-guide.md](branding/style-guide.md) for colors, typography, and component specifications.

## License

[MIT License](LICENSE.txt)
