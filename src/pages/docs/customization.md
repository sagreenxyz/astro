---
layout: ../../layouts/MarkdownLayout.astro
title: Customization Guide
description: Learn how to customize your Astro site
date: 2024-01-22
---

## Customizing Your Site

This guide will help you customize your Astro markdown site to match your needs and preferences.

## Configuration

### Site Configuration

Edit `astro.config.mjs` to configure your site:

```javascript
export default defineConfig({
  site: 'https://example.com',
  base: '/my-site',
});
```

### Package.json

Update your `package.json` to set your project name and details.

## Styling

### Global Styles

Global styles are defined in `src/layouts/Layout.astro`. You can modify:

- Color scheme
- Typography
- Spacing
- Layout dimensions

### Component Styles

Each `.astro` component can have scoped styles:

```astro
<style>
  h1 {
    color: blue;
  }
</style>
```

### CSS Variables

The site uses CSS variables for theming:

```css
:root {
  --accent: 136, 58, 234;
  --accent-light: 224, 204, 250;
  --accent-dark: 49, 10, 101;
}
```

## Adding New Pages

### Static Pages

Create a new `.astro` file in `src/pages/`:

```astro
---
import Layout from '../layouts/Layout.astro';
---

<Layout title="My Page">
  <h1>Hello World</h1>
</Layout>
```

### Markdown Documents

Create a new `.md` file in `src/pages/docs/`:

```markdown
---
layout: ../../layouts/MarkdownLayout.astro
title: My Document
description: A brief description
date: 2024-01-22
---

## Content

Your markdown content here...
```

## Navigation

Update the navigation in `src/layouts/Layout.astro` to add new links:

```html
<nav>
  <a href="/docs">Documentation</a>
  <a href="/blog">Blog</a>
  <a href="/about">About</a>
</nav>
```

## Advanced Customization

### Adding Components

Create reusable components in `src/components/`:

```astro
---
interface Props {
  message: string;
}
const { message } = Astro.props;
---

<div class="alert">
  {message}
</div>
```

### Using Integrations

Add Astro integrations for extra functionality:

```bash
npm install @astrojs/tailwind
npx astro add tailwind
```

### Environment Variables

Create a `.env` file for environment-specific configuration:

```
PUBLIC_API_URL=https://api.example.com
```

## Tips

1. Keep your layout consistent across pages
2. Use meaningful frontmatter for better organization
3. Organize content into logical directories
4. Test your site locally before deploying
5. Use semantic HTML for better accessibility

## Next Steps

- Explore Astro integrations
- Add search functionality
- Implement dark/light mode toggle
- Create custom components
- Set up continuous deployment

Happy customizing! 🎨
