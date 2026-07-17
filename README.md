# shahshlok.com

A hand-written static personal website built with HTML and CSS. There is no framework, package manager, build step, or runtime JavaScript.

## Local preview

From the repository root:

```sh
uv run python -m http.server 8000 --directory site
```

Then open `http://localhost:8000`.

## Add a blog post

1. Copy one of the existing folders in `site/blog/` to `site/blog/your-post-slug/`.
2. Update the title, description, canonical URL, article text, and draft status.
3. Add the post to `site/blog/index.html` and the homepage writing section.
4. When it is ready to publish, remove `noindex`, add truthful publication metadata, and add the URL to `site/sitemap.xml`.
5. Preview locally and check every link before committing.

## Cloudflare Pages

- Production branch: `main`
- Build command: `exit 0`
- Build output directory: `site`
- Canonical domain: `https://shahshlok.com`

The custom domain should be added through the Cloudflare Pages dashboard after the preview deployment is approved.
