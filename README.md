# tld-theme

A dark-first, monospace-forward Ghost theme for [thelaziest.dev](https://thelaziest.dev). Built with JetBrains Mono, Inter, Alpine.js, and Tailwind CSS on top of Ghost's Solo theme.

# Prerequisites

This theme requires the following Ghost configuration:

```
privacy__useStructuredData=false
```

This disables Ghost's built-in Open Graph / Twitter Card / JSON-LD output from `{{ghost_head}}`, allowing the theme to manage its own structured data. The theme outputs all necessary meta tags via the `meta-tags` partial, including dynamically generated social card images powered by [Microlink Cards](https://cards.microlink.io).

Without this setting, Ghost will output duplicate `og:image` tags that conflict with the theme's generated social cards.

`{{ghost_head}}` continues to handle Portal, search, Stripe, code injection, and other non-metadata functionality.

# Development

Styles are compiled using Gulp/PostCSS. You'll need [Node](https://nodejs.org/) and [Gulp](https://gulpjs.com) installed globally.

```bash
# Install dependencies
cd src && npm install

# Run build & watch for changes
npm run dev
```

Now you can edit `/assets/css/` files, which will be compiled to `/assets/built/` automatically.

```bash
# Package theme for upload
npm run zip
```

# Social Cards

Post pages automatically get dynamically generated social thumbnails via Microlink Cards. The card template matches the site's dark design:

- Background: `#0B0F14`
- Title: white JetBrains Mono bold
- Description: `#9BA6B2` Inter
- Accent: `#00FF88` green (brand color)

The card template is encoded in the `meta-tags` partial. To modify the card design, use the [Microlink Cards editor](https://cards.microlink.io/editor), update the query variables to match your theme, and replace the `p` parameter in the partial.

Non-post pages (homepage, tags, authors) fall back to the site cover image for `og:image`.

## Copyright & License

Based on [Solo](https://github.com/TryGhost/Solo) by Ghost Foundation - Released under the [MIT license](LICENSE).
