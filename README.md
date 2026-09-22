# Technovative Applications Website

Source files for the Technovative Applications marketing website: a static site built with plain HTML and CSS, with no frameworks and no build step.

## Folder structure

```
technovative/
├── README.md          ← this file
├── docs/              ← specifications and decisions
├── design/            ← reference exports from Figma (not part of the website)
└── site/              ← the website itself; this is the folder that gets deployed
    ├── index.html     ← one .html file per page
    ├── css/           ← stylesheets, including design tokens
    └── assets/
        ├── fonts/     ← self-hosted web font files (supplied separately; see below)
        ├── images/    ← photography and illustrations
        ├── icons/     ← interface icons (SVG)
        └── logos/     ← logo files (SVG)
```

### `docs/`
Written rules the site is built against: the grid, breakpoints, type scale, color palette, and a log of design and technical decisions. When the code and the docs disagree, the docs are the source of truth, and one of them needs updating.

### `design/`
Static exports of the Figma designs (PNG). They exist only for comparison while building and reviewing. Nothing in this folder is loaded by the website.

### `site/`
Everything the web server needs, and nothing else. To host the site, copy the contents of this folder to the server. No installation or compiling is required.

## Licensed fonts

The site uses Aeonik and Aeonik Fono, which are commercial typefaces. The font files are deliberately left out of this repository and are supplied with the handoff package. See `site/assets/fonts/README.md` for the expected filenames.

## Principles

- **No external requests.** Fonts, images, and scripts are all served from this folder. The site does not call third-party services, CDNs, or analytics.
- **Tokens before values.** Colors, font sizes, spacing, and grid measurements are defined once as CSS custom properties and referenced by name everywhere else.
- **Semantic, readable markup.** Class names describe what something is (`.site-header`, `.card`), not how it looks.
- **Accessible by default.** Target: WCAG 2.1 AA / Section 508 (to be confirmed with the client).
- **Minimal JavaScript.** It is used only where HTML and CSS can't do the job.

## Status

Brand assets added: logos, icons, and font documentation. Design tokens and specifications come next.
