# Astro Markdown Documentation Site

A modern, fast website built with [Astro](https://astro.build) for holding and presenting markdown documents. Features a clean design, built-in markdown support, and room for future expansion.

## 🚀 Features

- **📝 Markdown Support** - Write your content in Markdown with full syntax support
- **⚡ Lightning Fast** - Built with Astro for optimal performance
- **🎨 Beautiful Design** - Clean, modern interface with a professional look
- **📱 Responsive** - Works great on all devices
- **🔧 Easy to Customize** - Simple structure and clear code
- **🚀 Ready to Deploy** - Deploy anywhere that supports static sites

## 📁 Project Structure

```
/
├── public/              # Static assets (favicon, images)
├── src/
│   ├── layouts/         # Page layouts
│   │   ├── Layout.astro           # Main layout
│   │   └── MarkdownLayout.astro   # Layout for markdown documents
│   └── pages/           # Pages and routes
│       ├── index.astro            # Home page
│       ├── about.astro            # About page
│       └── docs/                  # Documentation directory
│           ├── index.astro        # Docs listing page
│           ├── getting-started.md # Sample markdown doc
│           ├── astro-features.md  # Sample markdown doc
│           └── customization.md   # Sample markdown doc
├── astro.config.mjs     # Astro configuration
├── package.json         # Project dependencies
└── tsconfig.json        # TypeScript configuration
```

## 🧞 Commands

All commands are run from the root of the project, from a terminal:

| Command                | Action                                           |
| :--------------------- | :----------------------------------------------- |
| `npm install`          | Installs dependencies                            |
| `npm run dev`          | Starts local dev server at `localhost:4321`      |
| `npm run build`        | Build your production site to `./dist/`          |
| `npm run preview`      | Preview your build locally, before deploying     |
| `npm run astro ...`    | Run CLI commands like `astro add`, `astro check` |

## 📝 Adding New Documents

To add a new markdown document:

1. Create a new `.md` file in `src/pages/docs/`
2. Add frontmatter at the top:

```markdown
---
layout: ../../layouts/MarkdownLayout.astro
title: Your Document Title
description: A brief description
date: 2024-01-22
---

## Your content here...
```

3. Write your content in Markdown
4. Your page will automatically be available at `/docs/your-filename`

## 🎨 Customization

- **Colors and Theme**: Edit `src/layouts/Layout.astro` to modify CSS variables
- **Navigation**: Update the nav section in `src/layouts/Layout.astro`
- **Layout**: Modify `src/layouts/MarkdownLayout.astro` for document styling
- **Configuration**: Edit `astro.config.mjs` for site-wide settings

## 🚀 Deployment

This site can be deployed to any static hosting service:

- **Vercel**: Connect your repo and deploy automatically
- **Netlify**: Drag and drop the `dist/` folder after `npm run build`
- **GitHub Pages**: Use GitHub Actions for automatic deployment
- **Cloudflare Pages**: Connect your repo for automatic builds

Build command: `npm run build`  
Output directory: `dist`

## 📚 Learn More

- [Astro Documentation](https://docs.astro.build)
- [Astro Discord Community](https://astro.build/chat)
- [Markdown Guide](https://www.markdownguide.org/)

## 🛠️ Future Expansion Ideas

- Add search functionality
- Implement tags/categories
- Add table of contents
- Dark/light mode toggle
- RSS feed for updates
- Comments system
- PDF export
- Multi-language support

## 📄 License

This project is open source and available for personal and commercial use.
