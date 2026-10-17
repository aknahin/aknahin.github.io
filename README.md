# Asrafuzzaman Khan Nahin — research profile

A Jekyll site using the [Hydejack](https://github.com/hydecorp/hydejack) theme (v9.2), deployed to GitHub Pages by `.github/workflows/pages.yml` on every push to `main`.

## Pages

- `index.md` — introduction and featured work
- `projects.md` — research projects
- `publications.md` — papers and manuscript status
- `contact.md` — email and academic profiles

Site settings and the sidebar menu are in `_config.yml`; the author card and social links are in `_data/authors.yml`. Custom CSS goes in `_sass/my-inline.scss` or `_sass/my-style.scss`.

The downloadable CV is in `assets/Asrafuzzaman-Khan-Nahin-CV.pdf`. Update the PDF and page text together when the record changes.

## Local preview

```sh
bundle install
bundle exec jekyll serve --livereload
```
