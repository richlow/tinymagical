# Tiny Magic

Personal blog and portfolio for [Rich Low](https://richlow.com) — documenting the journey of building small products.

## Stack

- **[Jekyll](https://jekyllrb.com/) 4.3** — static site generator
- **[Minima](https://github.com/jekyll/minima) 2.5** — base theme (extended with custom layouts)
- **[jekyll-feed](https://github.com/jekyll/jekyll-feed)** — RSS feed generation
- **Ruby / Bundler** — dependency management
- **Kramdown + GFM** — Markdown rendering

## Local development

**Prerequisites:** Ruby and Bundler installed.

```bash
bundle install
bundle exec jekyll serve
```

Then open [http://localhost:4000](http://localhost:4000).

## Project structure

```
├── _config.yml          # Site configuration (title, url, social usernames)
├── _layouts/            # Custom page layouts (default, post)
├── _posts/              # Blog posts (Markdown)
├── _data/
│   └── projects.yml     # Data file powering the "Tiny Products" list on the home page
├── assets/css/          # Global styles
├── index.markdown        # Home page
├── blog.html            # Blog listing, grouped by year
├── about.markdown        # About page
└── pomodoro.markdown     # Pomodoro product page
```

## Editing content

**Blog posts** — add a new Markdown file to `_posts/` following the `YYYY-MM-DD-title.markdown` naming convention. Front matter:

```yaml
---
layout: post
title: "Post title"
date: 2026-01-01
---
```

**Projects list** — edit `_data/projects.yml`. Each entry drives a card on the home page:

```yaml
- name: Pomodoro
  url: /pomodoro
  description: A simple Pomodoro timer.
```

## Deployment

The site is designed for **GitHub Pages** or any static host.

For GitHub Pages, swap the `Gemfile` dependency from `jekyll` to `github-pages` (instructions are commented in the `Gemfile`), then set `baseurl` and `url` in `_config.yml` to match your domain.

## License

MIT © 2026 Rich Low
