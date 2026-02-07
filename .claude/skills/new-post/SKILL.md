---
name: new-post
description: Create a new project blog post for cooldad.computer with proper frontmatter and structure.
argument-hint: [project-title]
allowed-tools: Write, Read, Bash
---

# Create New Blog Post

Create a new Jekyll blog post for cooldad.computer following the established project write-up format.

## Process

1. **Create a git branch** for the new post:
   - Format: `post/slugified-title`
   - Example: `post/my-cool-project`
   - Checkout the new branch before creating files

2. **Gather information** - Ask the user for:
   - Project title (used for filename and frontmatter)
   - Tagline (short phrase for the summary heading, e.g., "Dungeon Guide meets LLMs")
   - Description (2-3 sentences, max 280 chars)
   - Tags (2-5 lowercase tags)

3. **Generate the filename** using today's date and slugified title:
   - Format: `_posts/YYYY-MM-DD-slugified-title.md`
   - Example: `_posts/2026-02-07-my-cool-project.md`

4. **Create the post** using the template structure from `template.md` in this skill directory

5. **Open for editing** - After creating, let the user know they can fill in the sections

## Content Guidelines

From CLAUDE.md:
- Write in first person, conversational tone
- Be technically specific but accessible
- Embrace honest reflections about challenges
- Avoid marketing speak and buzzwords

## Frontmatter Rules

- `layout: post` (always)
- `title`: 3-8 words, descriptive but punchy
- `description`: 2-3 sentences, max 280 characters
- `date`: YYYY-MM-DD 12:00:00 format
- `tags`: 2-5 lowercase tags separated by commas
