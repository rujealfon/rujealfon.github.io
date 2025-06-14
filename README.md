# Ruje Alfon - Portfolio Website

A modern, responsive portfolio website built with Tailwind CSS and enhanced with GSAP animations.

## Features

- ✨ Modern design with Vue.js-inspired color palette
- 🎨 Tailwind CSS for styling
- 🎪 GSAP animations for smooth interactions
- 📱 Fully responsive design
- 🚀 Optimized for performance
- 🎯 SEO optimized with structured data

## Tech Stack

- **Runtime**: Bun (JavaScript runtime and package manager)
- **Styling**: Tailwind CSS v4.1.10 (Stable)
- **Build Tool**: PostCSS with @tailwindcss/postcss plugin via Bun
- **Animations**: GSAP (GreenSock Animation Platform)
- **Font**: Inter (same as Vue.js website)
- **Icons**: Font Awesome 6

## Development

### Prerequisites

- Bun (latest version)
  ```bash
  curl -fsSL https://bun.sh/install | bash
  ```

### Setup

1. Clone the repository:
```bash
git clone https://github.com/rujealfon/rujealfon.github.io.git
cd rujealfon.github.io
```

2. Install dependencies:
```bash
bun install
```

3. Start development with CSS watching:
```bash
bun run dev
```

This will watch for changes in your CSS and automatically rebuild the `dist/output.css` file using Bun and PostCSS.

### Building for Production

The CSS is automatically built and deployed via GitHub Actions on every push to the main branch using Tailwind CSS v4's new engine.

For local production builds:

```bash
bun run build
```

This creates an optimized CSS file in `dist/output.css` using Bun with the Tailwind CSS v4.1.10 PostCSS plugin.

### GitHub Actions Workflow

The project uses GitHub Actions with Bun to automatically:
- Build Tailwind CSS v4.1.10 on every push to main using Bun
- Deploy to GitHub Pages with the latest compiled CSS
- Ensure production CSS is always up-to-date

The workflow file is located at `.github/workflows/static.yml` and uses the official Bun setup action.

## Project Structure

```
├── .github/
│   └── workflows/
│       └── static.yml     # GitHub Actions workflow with CSS build
├── src/
│   └── input.css          # Source CSS with Tailwind v4 @theme configuration
├── dist/                  # Compiled CSS (generated by GitHub Actions)
│   └── output.css         # Production CSS file
├── fonts/                 # Custom fonts
├── icon/                  # Favicon and app icons
├── index.html            # Main portfolio page
├── cv.html               # CV/Resume page
├── postcss.config.js     # PostCSS configuration for Tailwind v4
├── package.json          # Dependencies and scripts
└── README.md             # This file
```

## Customization

### Colors

The color palette is defined using Tailwind CSS v4's new `@theme` directive in `src/input.css` and includes:

- **Vue.js colors**: `vue-green`, `vue-blue`
- **Nuxt-inspired palette**: `nuxt-dark`, `nuxt-accent`, `nuxt-surface`, etc.

### Fonts

The project uses Inter font family (same as Vue.js website) defined in the `@theme` block for optimal readability and modern appearance.

### Custom Styles

Additional custom styles and animations are defined in `src/input.css` alongside the Tailwind v4 theme configuration.

## Scripts

- `bun run dev` - Start development with CSS watching
- `bun run build` - Build production CSS (includes clean)
- `bun run build-css` - Build CSS with watching
- `bun run build-css-prod` - Build production CSS with Bun
- `bun run clean` - Remove dist directory

## Browser Support

This website supports all modern browsers including:
- Chrome/Edge (latest)
- Firefox (latest)
- Safari (latest)

## License

MIT License - feel free to use this as a template for your own portfolio!

## Contact

- **Email**: rujealfon@gmail.com
- **GitHub**: [github.com/rujealfon](https://github.com/rujealfon)
- **Website**: [rujealfon.github.io](https://rujealfon.github.io)