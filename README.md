# bishal

Personal site: essays and projects. Plain Jekyll, no theme, one stylesheet.

## Writing

- Essays go in `_posts/` as `YYYY-MM-DD-slug.md` and are published at `/posts/slug/`.
- Front matter: `title`, `date`, optional `tags`, and `math: true` for posts with LaTeX.
- Math: `$...$` is inline, `$$...$$` is display. It's rendered by KaTeX, which only loads on posts with `math: true`.
- Tables, images, footnotes and `<details>` blocks work as normal Markdown/HTML.

## Projects

Edit `_data/projects.yml`. `featured: true` puts a project on the home page, and `show: false` hides it.

## Settings

`_config.yml` holds the title, the contact email (defined once), and social handles.

## Local preview

```sh
bundle install
bundle exec jekyll serve --livereload
```

## Deploy

Pushing to `main` builds and deploys through `.github/workflows/pages-deploy.yml`.

The site is served at https://bishal.co.uk. The domain is set in Settings → Pages (no `CNAME` file is needed when deploying with Actions), and DNS lives in Cloudflare.
