# MuseRank Documentation

The official end-user documentation for [MuseRank](https://app.muserank.com) — the AI content and SEO platform. This site is built with [Mintlify](https://mintlify.com) and published from this repository.

## Structure

Content is written in MDX and organized into four tabs, configured in `docs.json`:

| Tab | Folder | Covers |
| --- | --- | --- |
| **Get Started** | `/` | Introduction, core concepts, quickstart, onboarding |
| **Guides** | `guides/` | Keyword research, topical maps, content creation, planning & automation, analytics, account |
| **Publishing & Integrations** | `integrations/` | WordPress, Shopify, Webflow, Framer, Ghost, Notion, GitHub, webhooks, Google Search Console |
| **Help** | `help/` | Troubleshooting, FAQ, support |

Branding assets live in `logo/` (`light.svg`, `dark.svg`) and `favicon.svg`. Global settings, navigation, colors, navbar, and footer are all defined in `docs.json`.

## Develop locally

Install the Mintlify CLI and run the dev server from the repository root (where `docs.json` lives):

```bash
npm i -g mint
mint dev
```

The site is served at `http://localhost:3000`. Edits to MDX files and `docs.json` hot-reload.

To check for broken internal links before publishing:

```bash
mint broken-links
```

## Editing content

- Pages are `.mdx` files. Each starts with frontmatter (`title`, `description`).
- Add a new page by creating the file and listing its path (without the `.mdx` extension) in the relevant group inside `docs.json`.
- Use Mintlify components such as `Card`, `CardGroup`, `Steps`, `Accordion`, `Note`, `Tip`, and `Warning` for consistent formatting.

## Publishing

Changes merged to the default branch are deployed automatically by Mintlify.

## License

© MuseRank. All rights reserved.
