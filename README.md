# CamBio — project site

Source for the CamBio showcase site, published with GitHub Pages at
**https://will-raymond.github.io/cambio/**.

CamBio is a library of voice-controlled AI lab assistants for automated lab
equipment (OpenTrons Flex/OT-2, I.DOT, Bambu printers, ...), coordinated by a
director agent. This repository contains **only the showcase site**, not the
application code.

## Stack

- [Jekyll](https://jekyllrb.com/), built and deployed by GitHub Actions
  (`.github/workflows/jekyll.yml`) on every push to `main`
- [Minimal Mistakes](https://mmistakes.github.io/minimal-mistakes/) via the
  `minimal-mistakes-jekyll` gem, with local CSU-branded overrides in `_sass/`,
  `_layouts/` and `_includes/` (skin: `_sass/minimal-mistakes/skins/_csu.scss`)

## Structure

```
_config.yml          # site config, theme, baseurl
index.md             # splash landing page
_pages/              # Capabilities (agents.md), Roadmap, Experiments,
                     # Publications, Media, Contact/About
_data/navigation.yml # top navigation
_sass/ _layouts/ _includes/  # theme overrides
assets/images/       # hero image and media
```

## Local preview

```bash
bundle install
bundle exec jekyll serve --baseurl ""
# → http://localhost:4000
```

(Requires Ruby + Bundler.)
