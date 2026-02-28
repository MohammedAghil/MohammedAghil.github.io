# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Overview

A static personal portfolio website hosted on GitHub Pages. No build system, package manager, or server-side code — just plain HTML, CSS, and CDN-loaded libraries.

## Stack

- **Bootstrap 4.5.2** (CDN) for layout and components
- **jQuery 3.5.1** + **Popper.js 1.16.0** (CDN) as Bootstrap dependencies
- **`css/main.css`** for custom styles layered on top of Bootstrap
- **`images/`** holds profile photo and company logos used in `index.html`

## Structure

The entire site is a single page (`index.html`) with three anchor-linked sections:
- `#about` — profile photo + bio
- `#skills` — skill badges
- `#exp` — experience cards (Bootstrap `.card.bg-info`)

No JavaScript beyond what Bootstrap/jQuery require. No local dependencies to install.

## Development

Open `index.html` directly in a browser — no local server needed. For live-reload during editing, any static file server works:

```bash
python3 -m http.server 8080
# or
npx serve .
```

## Deployment

Pushing to the `main` branch on GitHub automatically deploys to GitHub Pages.
