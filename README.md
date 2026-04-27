# Omnier documentation

This repository powers the public **Omnier** docs (Mintlify). Content is MDX in the repo root; site config is [`docs.json`](./docs.json).

**Pages (in order):** [What is Omnier?](./index.mdx) (home) → [Getting started](./getting-started.mdx). Written for founders and sales users, not developers.

## Local preview

[Install the Mintlify CLI](https://www.npmjs.com/package/mint), then from this directory:

```bash
npm i -g mint
mint dev
```

Open the URL shown (commonly `http://localhost:3000`).

## Authoring

- Add or edit `.mdx` files.
- Register each page in `docs.json` under `navigation` → `tabs` → `groups` → `pages` (use the path without `.mdx`).

## Publishing

Connect this GitHub repository in the [Mintlify dashboard](https://dashboard.mintlify.com) and push to the deployment branch. Builds run automatically on push.

## Styling

Docs follow the product palette from the landing app: **Inter**, background **`#F8F7F6`**, primary accent **`#4A6B5C`** (see `docs.json` and [`globals.css`](../landingpage/frontend/src/app/globals.css) in the monorepo).
