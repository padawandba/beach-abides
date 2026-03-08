# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Static website for "The Beach Abides" — an Airbnb vacation rental property in St. Augustine, FL. Hosted via GitHub Pages at beachabides.com (configured via CNAME).

## Architecture

This is a single-page static site with no build system, no dependencies, and no framework:

- `index.html` — The entire site: markup, CSS (inline `<style>`), and JS (inline `<script>`)
- `images/` — Static assets (PNG/JPG) referenced by the HTML
- `CNAME` — GitHub Pages custom domain config

All styles are embedded in a `<style>` block in the `<head>`. All JavaScript (smooth scrolling, active nav highlighting, mobile menu toggle) is in a `<script>` block at the end of `<body>`.

## Development

No build or install step. Open `index.html` in a browser to preview. Deploy by pushing to `main` (GitHub Pages).

## Key Conventions

- Fonts loaded from Google Fonts: PT Sans, Merriweather, Comfortaa
- Navigation uses anchor links to `<section id="...">` elements
- Mobile responsive via media query at 768px breakpoint
- Images use classes `section-img` and `section-img--wide` for layout
