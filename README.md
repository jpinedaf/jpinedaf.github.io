# Personal webpage

This site is built with [Jekyll](https://jekyllrb.com/) using the
[Minimal Light](https://github.com/yaoyao-liu/minimal-light) theme (via
`remote_theme`), as adapted in
[qizhang94/qizhang94.github.io](https://github.com/qizhang94/qizhang94.github.io).

Content is split across the Home, Research, CV, Contact, and Publications pages, with the publication list sourced from
[`_data/publications.yml`](_data/publications.yml).

## Building locally

```sh
bundle install
bundle exec jekyll serve
```

## Deployment

The site is built and deployed to GitHub Pages via GitHub Actions
(see [`.github/workflows/pages.yml`](.github/workflows/pages.yml)) on every
push to `master`. In the repository settings, GitHub Pages must be configured
with **Source: GitHub Actions**.
