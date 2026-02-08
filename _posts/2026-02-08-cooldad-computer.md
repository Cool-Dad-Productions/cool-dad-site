---
layout: post
title: "cooldad.computer"
description: You're looking at it!
date: 2026-02-08 12:00:00
tags: static-site, jekyll, github-pages
---

## cooldad.computer: You're looking at it!

A few weeks ago, I bought some t-shirts from an online store. I would get free shipping with a third shirt, so I found a brown shirt "Cool Dad" embroidered across the front. It seemed just dorky and ironic enough to get the appropriate eye roll from my twelve year old. 

But when it arrived, I realized the actual product was just cheap vinyl letters. The shirt quickly went from quirky dorky to straight bad-taste dorky. (The other two shirts were spot on perfect, so 2 out of 3 ain't bad.)

My wife and daughter also pointed out buying a shirt that said "Cool Dad" for myself was weird. Fair point!

At the same time, I've been spending time building some side projects and I realized I wanted to capture my thoughts about what I learned. This helps me stay focused and iterate quickly on what I'm learning. I also wanted to push myself to learn in public.

I needed a way to rescue the Cool Dad shirt debacle and meet these learning goals. I spun up a Github pages site and used the shirt as the basis for the styling. And so [cooldad.computer](https://cooldad.computer) was born! I don't think this helps me recover from the awful shirt purchase, it just digs me deeper, but as a learning tool I've been very happy!

## Learning Goals
- Capture learnings from my side projects and feed those back into future projects
- Keep track of all these projects
- Give myself a place to experiment and learn without constraints

## Links
- [Repo](https://github.com/Cool-Dad-Productions/cool-dad-site)
- [Site](https://cooldad.computer/)

## Stack/Tooling
- Github pages for hosting
- SASS styling
- Font Awesome for icons
- Favicon.io for favicon generation
- Google Tag Manager for analytics
- ChatGPT for initial styling
- Claude Code for style guide, style, and other updates

## Main Takeaways

Github Pages continues to be my favorite way to spin up a static site. There may be better options, but having a chosen platform reduces barriers to starting projects.

Claude did well with my prompts that instructed it to iterate until a quality metric was hit. This was like dipping a toe into some more complex iterative workflows like [Ralph](https://github.com/snarktank/ralph).

## Relevant Prompts

These were the Claude prompts used to pick a Jekyll template and generate a style guide.

### Picking a theme

```
I am a software engineer and I have the domain cooldad.computer.  I want to host a personal portfolio site of side projects at this domain using Github Pages. The projects I make are one off coding projects. They are usually whimsical and are purpose built to help me learn or to test a new technology or approach.

I need a template for this site. I'd like to use something free.

Constraints:
* The template should be free
* The tone should be whimsical, but keep with an ironic technology/computer/nerd aesthetic.
* the site will be hosted on Github pages
* I am comfortable making basic styling changes (colors, fonts, images), but don't want to spend a lot of time rewriting the template to make it work
* The logo I use has a primary background color of #6B4A3A, font color of #CFEFF2, and uses the Libre Baskerville font (regular 400 normal)

You are a senior designer with 10 years experience designing websites. I am enlisting your help with picking the initial them. 

 I want you to explain my use case, tell me how you will evaluate templates, and tell me how you will find them. Once you have a plan, then I want you to find 5 templates, evaluate them using your criteria, and sort them from best to worst. Provide a bulleted summary with each template explaining how it fared in the evaluation.
```

### Developing a style guide

```
ok, after weighing all the options, I'm going to start with the first option: "Jekyll Theme Console". This may be minimal, but it's a good start for a lightweight afternoon project. 

Next I will need you as a Senior Designer to create a style guide for me.

First tell me how you would evaluate a style guide for a portfolio site. Tell me what topics should exist should be covered. Then create an outline of a style guide and ask me for feedback. Once we agree on the outline, I want you to populate the style guide with your proposed styling.

Finally, I want you to evaluate your style guide using your criteria on a scale of 1 to 100, with 100 being perfect and 1 being completely undesirable. If your score is below 90, create and execute a plan to correct it. Continue this until the style guide evaluation is above 90. 

Finally, print the final style guide in markdown format.

Some existing assets:
* I attached a jpeg that can be the basis of the style guide
* the logo background color is #6B4A3A
* the logo font color is #CFEFF2
* the font is "Libre Baskerville font (regular 400 normal)"
```

## Reflections

I've spun up a few Github Pages sites, so choosing that as a platform was an easy choice. I leaned heavily on AI for creating style guides and styling the site itself. I included some of the most relevant prompts above.

I set up apex domain routing and a `cname` for the `www` subdomain. Github documents this well; it was a simple copy-paste. Setting up other project-specific subdomains is trivial and doesn't interfere with the apex DNS settings.

The style guide approach I took is a great pattern for apps and sites built with AI. It creates a human readable, but structured natural language definition of styling that coding agents can consume and conform to. This is a pattern I want to extend into other areas of code.

I created a Claude skill to add new pages. In the past, I've created bash scripts to do this, but wanted to experiment. Obviously this creates vendor lock in, though it would be easy to convert the skill to some other markdown based AI interface.

I do worry a bit about usage/token consumption with this skill approach. I think my next step will be to create a well documented bash script, that way Claude just needs to know the interface and execute the script. Properly done, that should reduce token usage a bit. After all, [tokens are the new oil](https://tidyfirst.substack.com/p/tokens-the-new-oil).
