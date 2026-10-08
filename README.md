# joey-site

The public site behind **joey-go.com** — currently Joey's privacy policy and terms of service.

## 🔴 Do not edit the HTML in this repo

Every `.html` file here is **generated**. Editing one works until the next build, then
the change is gone.

The source of truth is the Markdown in the private `joey-app` repo, under `legal/`.

## Changing a document

```
1. edit joey-app/legal/*.md
2. cd joey-app && node scripts/build-legal-site.js
3.                node scripts/verify-legal-site.js
4. commit joey-app   (the source changed)
5. commit + push joey-site   (the site changed)
```

Two repos, two commits — that is deliberate. It maps onto "the source changed,
so the site changed", which is why it is easy to remember.

## Status of these documents

They are **drafts that have not been reviewed by a lawyer** and are not binding.
Anything in `[square brackets]` is a legal or business decision that has not been
made yet. Every page carries a banner saying so.

`noindex` is set on every page on purpose, so drafts do not reach search engines.
Remove it after legal review.

## Setup

GitHub Pages: **main branch, / (root)**. Custom domain and the Namecheap DNS
records are documented in `SITE_DEPLOY.md` in the joey-app repo.
