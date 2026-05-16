# Genshin Impact Game Guide Website — Design Spec

**Date:** 2026-05-17
**Status:** approved

## Overview

English-language Genshin Impact game guide website with 15 long-form articles, deployed via GitHub Pages as pure static HTML/CSS.

## Architecture

```
root/
  index.html            Homepage with article cards + category nav
  css/
    style.css            Single stylesheet, dark Genshin-accented theme
  guide/
    linnea-build.html    Article 1
    zibai-build.html     Article 2
    ...                  Articles 3-15
```

No JavaScript. No external dependencies. No build step.

## Design

- **Theme:** Dark (bg `#1a1a2e`), gold accents (`#d4a574`)
- **Homepage:** Filterable article cards by category (Build Guide, Meta, F2P, Tier List)
- **Article page:** Breadcrumb, centered content column (max-width 720px), sidebar with related articles
- **Typography:** System font stack, clear heading hierarchy

## Content

15 pre-written articles, ~500 words each. Categories:

| Category | Count |
|----------|-------|
| Build Guide | 5 (Linnea, Zibai, Nicole, Lorn, Weapons) |
| Meta/Magecraft | 4 |
| F2P/Starter | 3 |
| Tier List/Polls | 3 |

## Deployment

GitHub Pages on repo `12312131/Genshin-Impact`, served at `https://12312131.github.io/Genshin-Impact/`.
