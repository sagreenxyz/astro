---
layout: ../../layouts/MarkdownLayout.astro
title: Astro Features
description: Learn about the powerful features of Astro
date: 2024-01-21
---

## Why Astro?

Astro is a modern web framework designed for speed and performance. It's built with content-focused websites in mind, making it perfect for documentation sites, blogs, and portfolios.

## Key Features

### Zero JavaScript by Default

Astro ships zero JavaScript by default. This means your site loads incredibly fast because there's no unnecessary JavaScript being sent to the browser.

### Component Islands

Astro pioneered the concept of "Islands Architecture" - you can use components from any framework (React, Vue, Svelte) only where you need them, keeping the rest of your site fast and lightweight.

### Built-in Markdown Support

Astro has first-class support for markdown and MDX. You can:

- Write content in markdown files
- Use frontmatter for metadata
- Import and use components in markdown
- Create custom layouts for markdown pages

### Content Collections

Organize your content with Astro's Content Collections API:

```javascript
import { getCollection } from 'astro:content';

const docs = await getCollection('docs');
```

### Optimized for Performance

Astro automatically:

- Optimizes images
- Minimizes CSS
- Prefetches links
- Builds static HTML

## File-Based Routing

Astro uses file-based routing, making it intuitive to create new pages:

- `src/pages/index.astro` → `/`
- `src/pages/about.astro` → `/about`
- `src/pages/docs/guide.md` → `/docs/guide`

## Styling Options

You can use any styling approach you prefer:

- Scoped CSS in `.astro` files
- CSS preprocessors (Sass, Less)
- CSS frameworks (Tailwind, Bootstrap)
- CSS-in-JS libraries

## Deployment

Astro sites can be deployed anywhere:

- Vercel
- Netlify
- GitHub Pages
- Cloudflare Pages
- Any static hosting service

## Learn More

To dive deeper into Astro:

- Visit the [official documentation](https://docs.astro.build)
- Join the [Astro Discord community](https://astro.build/chat)
- Explore [Astro themes](https://astro.build/themes)

Happy building! 🎉
