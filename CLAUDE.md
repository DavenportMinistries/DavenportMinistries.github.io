# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Purpose

Davenport Ministries LLC's central public website, hosted at davenportministries.com via GitHub Pages. Serves as the org's digital home base: validates the business on Facebook and other platforms, links out to active projects, and provides general public-facing information. Audience is anyone looking up the organization — potential partners, app users, or platform verifiers.

## Tech Stack

- **Generator**: Jekyll (GitHub Pages native — zero build config, no CI needed)
- **Hosting**: GitHub Pages with custom domain (CNAME: davenportministries.com)
- **Styling**: Minimal CSS (no framework initially — keep it light)
- **Content**: Markdown + Liquid templates

Rationale: Jekyll was chosen because it's natively supported by GitHub Pages, requires no build pipeline, and fits the minimal-footprint goal of the site at this stage.

## External Integrations

- **Facebook Business Manager**: Site URL used to verify business domain ownership
- **fellowship-app.com**: Linked project (Davenport Ministries app)
- **sdamatch.app**: Linked project (SDA Match app)

## Architecture

Single-page Jekyll site (initially `index.html` or `index.md`). Sections:
- **About**: Brief description of Davenport Ministries LLC — what the org is and does
- **Projects**: Cards or list of active projects with name, short description, and link

Keep the structure flat — no complex layouts, collections, or plugins until genuinely needed. Add new projects as simple entries in the Projects section.

## Dev Commands

```bash
# Install Jekyll locally (one-time)
gem install bundler jekyll

# Serve locally with live reload
bundle exec jekyll serve

# Build static output
bundle exec jekyll build
```

> Note: GitHub Pages builds and deploys automatically on push to `main`. Local serving is optional.

## Doc Discipline

All code changes that affect documented behavior (site structure, new projects, integrations, stack changes) must include a corresponding update to CLAUDE.md, README.md, or docs/planning.md in the same commit. Do not ship undocumented changes.
