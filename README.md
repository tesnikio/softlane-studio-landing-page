# Softlane Studio Landing Page

A beautiful, modern landing page for Softlane Studio - a venture and product studio. Built with Astro and Tailwind CSS, deployed on GitHub Pages.

## Tech Stack

- [Astro](https://astro.build/) - Static site generator
- [Tailwind CSS](https://tailwindcss.com/) - Utility-first CSS framework
- [Lucide Icons](https://lucide.dev/) - Beautiful icon library
- [GitHub Pages](https://pages.github.com/) - Free hosting

## Getting Started

### Prerequisites

- Node.js 18 or later
- npm or yarn

### Installation

```bash
# Install dependencies
npm install

# Start development server
npm run dev

# Build for production
npm run build

# Preview production build
npm run preview
```

## Deployment to GitHub Pages

This project is configured for automatic deployment to GitHub Pages using GitHub Actions.

### Setup Steps:

1. **Update the Astro config** - Edit `astro.config.mjs` and update the `site` and `base` values:
   ```js
   export default defineConfig({
     integrations: [tailwind()],
     site: 'https://YOUR-USERNAME.github.io',
     base: '/YOUR-REPO-NAME',
   });
   ```
   
   If deploying to the root (e.g., `username.github.io`), set:
   ```js
   site: 'https://YOUR-USERNAME.github.io',
   base: '/',
   ```

2. **Enable GitHub Pages** - Go to your repository Settings → Pages → Source → Select "GitHub Actions"

3. **Push to main branch** - The deployment workflow will automatically build and deploy your site

## Project Structure

```
/
├── public/             # Static assets (favicon, robots.txt)
├── src/
│   ├── components/     # Astro components
│   ├── layouts/        # Page layouts
│   ├── pages/          # Page routes
│   └── styles/         # Global CSS
├── astro.config.mjs    # Astro configuration
├── tailwind.config.mjs # Tailwind configuration
└── package.json
```

## License

All rights reserved © Softlane Studio
