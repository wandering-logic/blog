# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a static blog for wanderinglogic.com. There is no build system or static site generator—HTML files are edited directly.

## Structure

- `docs/` - Published site served by GitHub Pages
  - `index.html` - Main page containing all blog posts
  - `css/style.css` - Site styling (Georgia font, cream background #fff9ec)
  - `images/` - All images including branding (big-ol-shoe.png)
  - `case-grounding/`, `enclosure-choices/` - Individual post pages (legacy URLs)
  - `CNAME` - Custom domain configuration (wanderinglogic.com)
  - `.nojekyll` - Disables Jekyll processing

## Adding New Posts

Add new `<article>` elements to `docs/index.html` inside `<main>`. Posts are ordered newest-first. Each article follows this structure:

```html
<article>
  <h1>Post Title</h1>
  <p><time datetime="YYYY-MM-DD">Month DD, YYYY</time></p>
  <!-- post content -->
</article>
```

## Previewing

Open `docs/index.html` directly in a browser, or use any local HTTP server:

```bash
cd docs && python3 -m http.server 8000
```
