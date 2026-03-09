# Chirpy Editorial Starter

A polished Jekyll starter built on top of the official Chirpy ecosystem:
`jekyll-theme-chirpy`, bootstrapped from `chirpy-starter`.

It keeps the Chirpy layout model, but adds:

- a refined editorial visual layer
- local web-font hosting
- SVG sidebar icons
- a cleaner archive layout
- a reading-first typography system

## What Is Included

- `jekyll-theme-chirpy` as the base theme
- the official Chirpy starter layout model and deployment flow
- local overrides in `_includes`, `_layouts`, and `assets/css`
- starter defaults in `_config.yml`
- official demo overrides in `_config.demo.yml`
- local web fonts in `assets/fonts`
- font license notices in `assets/fonts/LICENSES.md`
- a live Cloudflare Pages demo at `https://zong-liang-blog-starter.pages.dev`
- a few example posts and placeholder content

## Quick Start

1. Install Ruby and Bundler.
2. Run:

```powershell
bundle install
bundle exec jekyll serve --livereload
```

3. Open `http://127.0.0.1:4000/`.

## Live Demo

- `https://zong-liang-blog-starter.pages.dev`
- Built with `_config.yml` + `_config.demo.yml`

## Use This As A Starter

1. Click `Use this template` on GitHub, or fork the repository if you want to keep the full history.
2. Update `_config.yml`:
   - `title`, `tagline`, `description`, and `url`
   - `baseurl` only if you will publish under a subpath
   - `github.username`
   - `social.name`, `social.links`, and `avatar`
3. Replace the placeholder content in `_posts` and `_tabs/about.md`.
4. Replace the default avatar and favicon set in `assets/img`.
5. Push to `main`.
6. Deploy with your preferred static host.
7. The public demo in this repository uses Cloudflare Pages with:
   - build command: `BUNDLE_WITHOUT=development:test bundle exec jekyll build --config _config.yml,_config.demo.yml`
   - build output directory: `_site`
   - environment variable: `RUBY_VERSION=3.3.10`

## Config Layers

- `_config.yml` is the starter default that fork users should edit
- `_config.demo.yml` is only for the official hosted demo
- Local starter preview: `bundle exec jekyll serve --livereload`
- Local demo preview: `bundle exec jekyll serve --livereload --config _config.yml,_config.demo.yml`

## First Things To Replace

- `title`, `tagline`, `description`, `url` in `_config.yml`
- `baseurl` if you are publishing to a project site path
- `github.username`
- `social.name`, `social.links`
- `avatar`
- `comments` and `analytics`
- sample posts in `_posts`
- text in `_tabs/about.md`

## Font System

This starter uses local web fonts and does not depend on Google Fonts:

- UI sans: `Source Sans 3 Variable` + `Noto Sans SC Variable`
- Reading serif: `STIX Two Text Variable` + `Noto Serif SC Variable`
- Code mono: `JetBrains Mono Variable`

Font entry points:

- `assets/css/fonts.css`
- `assets/fonts`
- `assets/fonts/LICENSES.md`
- `assets/fonts/OFL-1.1.txt`
- `_includes/metadata-hook.html`
- `_data/origin/cors.yml`

## Font Licenses

This starter redistributes self-hosted font binaries.

- Family notices and provenance live in `assets/fonts/LICENSES.md`
- The shared SIL Open Font License 1.1 text lives in `assets/fonts/OFL-1.1.txt`

If you remove or replace any vendored font files, update both of those files in the same change.

## Upstream Credits

This repository is a small customization of Chirpy rather than an independent
theme.

- Theme: `jekyll-theme-chirpy` by Cotes Chung and contributors
- Bootstrap template: `chirpy-starter` by Cotes Chung and contributors
- Upstream license: MIT
- Repository notice: `NOTICE.md`

## Structure

- `_includes/sidebar.html`: sidebar override with SVG icons
- `_includes/topbar.html`: mobile-aware topbar override
- `_layouts/archives.html`: simplified archive layout
- `assets/css/jekyll-theme-chirpy.scss`: main visual override layer

## Notes

- This is a starter, not a standalone theme fork.
- Upgrading Chirpy is still possible, but you should review local overrides after theme updates.
- The public demo is hosted on Cloudflare Pages, and GitHub Pages is not part of the active deployment flow.
