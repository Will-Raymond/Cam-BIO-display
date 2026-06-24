# CamBio — project site

Source for the CamBio showcase site, published with GitHub Pages at
**https://cdsnow.github.io/cambio/**.

CamBio is a voice-controlled lab assistant for the OpenTrons Flex robot. This
repository contains **only the marketing/landing site** — not the application
code.

## Stack

- [Jekyll](https://jekyllrb.com/) (built natively by GitHub Pages — no Actions)
- [Minimal Mistakes](https://mmistakes.github.io/minimal-mistakes/) theme via `remote_theme`

## Structure

```
_config.yml          # site config, theme, baseurl
index.md             # splash landing page
_pages/              # Features, Roadmap, About
_data/navigation.yml # top navigation
assets/images/       # hero image and media
```

## Local preview

```bash
bundle install
bundle exec jekyll serve --baseurl ""
# → http://localhost:4000
```

(Requires Ruby + Bundler. GitHub Pages builds the published site automatically
on every push to `main`.)
