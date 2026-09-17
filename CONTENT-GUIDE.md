# Updating the RFMIP website — a guide for co-chairs

This is a short guide for adding or editing content on the RFMIP website
without needing to know Jekyll, Ruby, or the command line. Everything below
can be done from the GitHub website in a browser.

For deeper technical customization (theme colors, layout, config), see
[`CUSTOMIZE.md`](CUSTOMIZE.md) instead — this guide only covers day-to-day
content edits.

## How editing works, in short

The site is built from plain text files in this repository. When a change is
merged into the `main` branch, GitHub Pages automatically rebuilds and
publishes the live site within a minute or two — there is no separate
"publish" step.

To edit a file on GitHub without installing anything:

1. Open the file in this repository on github.com.
2. Click the pencil icon ("Edit this file") in the top right.
3. Make your change.
4. Scroll down, add a short description of what you changed, and choose
   **"Create a new branch for this commit and start a pull request."**
5. Open the pull request. Ask a co-chair (or anyone with write access) to
   glance at it, then merge it.

Using a pull request instead of committing straight to `main` means someone
can catch a typo or a broken link before it goes live, and it's easy to
revert if something looks wrong after publishing. For a trivial fix (e.g. a
typo), committing directly to `main` is also fine.

## Add a news item

News posts live in [`_news/`](_news) as one Markdown file per item, named
`announcement_N.md`.

To add one: copy the most recent file (e.g. `_news/announcement_4.md`) as a
template, rename it to the next number, and edit:

```markdown
---
layout: post
title: Your headline here
date: 2026-08-26 00:00:00-00
inline: false
related_posts: false
---

Body text of the announcement, in Markdown. Links look like
[this](https://example.com).
```

- `title` — shows as the headline on the About page and News listing.
- `date` — controls sort order (newest first). Keep the time/timezone
  suffix (`00:00:00-00`) as in existing posts.
- `inline: false` — keep this; it gives the post its own headline instead of
  folding it into a single line.
- The body below the `---` block is standard Markdown.

## Edit the About page (project description, co-chairs)

The homepage content is [`_pages/about.md`](_pages/about.md). The text below
the front-matter block (between the `---` lines and the end of the file) is
plain Markdown — edit it directly. This is also where the co-chair list and
the four RFMIP2.0 science questions live.

## Add or edit a publication

Publications are listed in [`_bibliography/papers.bib`](_bibliography/papers.bib)
in BibTeX format — one entry per paper. To add one, copy an existing entry as
a template:

```bibtex
@article{AuthorYear,
  title = {Full paper title},
  author = {Last, First and Last, First},
  journal = {Journal Name},
  volume = {19},
  number = {10},
  pages = {4447--4466},
  year = {2026},
  doi = {10.5194/xxxx},
  url = {https://doi.org/10.5194/xxxx},
  selected = {true}
}
```

- The `AuthorYear` key just needs to be unique in the file (e.g. `Kramer_2026`).
- `selected = {true}` features the paper prominently on the Publications page
  — leave it off (or set `false`) for a paper you want listed but not
  featured.
- `doi` and `url` are optional but recommended — they add a working link.

## Add or replace an image

Images (the logo, photos, figures) live in
[`assets/img/`](assets/img). Keep new images reasonably small — a few
hundred KB, not multiple MB — so the site stays fast to load. Reference an
image from a page with standard Markdown (`![alt text](/assets/img/file.png)`)
or, in a page's front matter, by filename alone (see `_pages/about.md` for
an example with the `profile.image` field).

## Getting help

For anything not covered here — site-wide settings, the visual theme,
navigation structure — see the upstream
[al-folio documentation](https://github.com/alshedivat/al-folio); we
removed our local copies of the template's own docs. Otherwise, ask
Chris.
