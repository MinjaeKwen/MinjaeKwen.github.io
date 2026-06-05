# MinjaeKwen.github.io

Personal academic portfolio website for Minjae Kwen.

**Live site**: [minjaekwen.com](https://minjaekwen.com)

## Stack

- **Jekyll** 3.9.3 — static site generator
- **GitHub Pages** — hosting & auto-deployment (push to `master` → live)
- **Netlify CMS** — web-based content editor at `/admin`
- **SASS** — modular stylesheets in `_sass/`

## Structure

```
_layouts/        # Page templates (default, page, post)
_includes/       # Shared partials (head.html)
_sass/           # SASS partials
css/             # SASS entry point (style.scss)
blog/_posts/     # Blog posts (YYYY-MM-DD-slug.md)
images/          # Image assets
files/           # PDFs (CV, papers, posters)
assets/uploads/  # CMS-managed uploads
research*.md     # Research project pages
```

## Local Development

```bash
git pull origin master   # Always pull first (Netlify CMS may have committed)
bundle exec jekyll serve # Serve at http://localhost:4000
```

## Deployment

Push to `master` → GitHub Pages builds and deploys automatically.

## License

MIT. See [LICENSE](LICENSE).
