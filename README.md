# gaudel.github.io

Sources of Romaric Gaudel's homepage, built by GitHub Pages (Jekyll) from Markdown.

## Where to edit

| Page | File |
|---|---|
| Home | `index.md` |
| Contact | `contact.md` |
| Students | `students.md` |
| Publications | `publications.md` |
| Talks | `talks.md` |
| Resume | `resume.md` |
| Teaching | `teaching/index.md` |
| ADM course | `teaching/adm.md` |
| INFO2 (ENS Rennes) | `teaching/info2-2022-2023.md`, `teaching/info2-2020-2021.md`, `teaching/info2-2019-2020.md`, `teaching/info2-2017-2019.md` (+ its two forums `teaching/info2-forum-*.md`) |
| Deep Learning (SV) | `teaching/deep-learning-sv.md` |

- Menu: `_data/navigation.yml`
- Page template: `_layouts/default.html`
- Style: `assets/css/style.css`
- Profile photo: put it at `assets/img/me.jpg` (shown on the home page as soon as the file exists).

To add a page, create `my-page.md` with this front matter, then add it to `_data/navigation.yml` if it should appear in the menu:

```yaml
---
layout: default
title: My page
permalink: /my-page/
---
```

## Local preview

```sh
bundle install
bundle exec jekyll serve
# then open http://localhost:4000
```

## Publishing

Push to `main`, then in the repository settings, *Pages* → *Build and deployment* → *Deploy from a branch* → `main` / `/ (root)`.
