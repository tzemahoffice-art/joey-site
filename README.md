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

They are published as Joey's current documents (STATUS.md §334). The lawyer's review
is still open; open questions live in joey-app (legal/QUESTIONS-LAWYER-ACCOUNTANT.html,
legal/PENDING-LAWYER.md), never on the site -- a check blocks any internal note here.

`noindex` is still set on every page -- remove it only when Orel decides.

## Setup

GitHub Pages: **main branch, / (root)**. Custom domain and the Namecheap DNS
records are documented in `SITE_DEPLOY.md` in the joey-app repo.
