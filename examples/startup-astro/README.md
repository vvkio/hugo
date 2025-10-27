# Startup Landing Page - Astro

A modern, responsive landing page template for startups built with Astro.

## Features

- **Modern Design**: Clean, professional design with gradient accents
- **Fully Responsive**: Mobile-first design that looks great on all devices
- **Smooth Animations**: Scroll animations and hover effects
- **SEO Friendly**: Semantic HTML with proper meta tags
- **Fast Loading**: Astro's zero-JS by default, optimized for performance
- **Easy to Customize**: Component-based architecture with clear structure
- **Type-Safe**: Built with TypeScript support

## Sections Included

1. **Navigation Bar**: Fixed navbar with smooth scroll navigation
2. **Hero Section**: Eye-catching hero with call-to-action buttons
3. **Features**: Showcase your product's key features with icons
4. **About**: Tell your company story with statistics
5. **Testimonials**: Display customer reviews and feedback
6. **Call-to-Action**: Encourage visitors to take action
7. **Footer**: Complete footer with links and contact information

## Getting Started

### Prerequisites

- Node.js 18+ installed
- npm, pnpm, or yarn package manager

### Installation

1. Navigate to this directory:
   ```bash
   cd examples/startup-astro
   ```

2. Install dependencies:
   ```bash
   npm install
   # or
   pnpm install
   # or
   yarn install
   ```

3. Run the development server:
   ```bash
   npm run dev
   # or
   pnpm dev
   # or
   yarn dev
   ```

4. Open your browser and visit:
   ```
   http://localhost:4321
   ```

### Building for Production

To build the static site for deployment:

```bash
npm run build
```

The generated site will be in the `dist/` directory.

To preview the production build:

```bash
npm run preview
```

## Customization

### Update Site Configuration

Edit `src/config.ts` to customize:
- Site title and description
- Company name and tagline
- Contact information
- Social media links

```typescript
export const siteConfig = {
  companyName: 'YourCompany',
  tagline: 'Your Custom Tagline',
  email: 'hello@yourcompany.com',
  // ... more settings
};
```

### Modify Components

All components are modular and located in `src/components/`:
- `Hero.astro` - Hero section
- `Features.astro` - Features grid
- `About.astro` - About section
- `Testimonials.astro` - Customer testimonials
- `CTA.astro` - Call-to-action
- `Footer.astro` - Footer
- `Navbar.astro` - Navigation bar

Edit any component to customize its content and structure.

### Styling

The main stylesheet is in `public/css/style.css`. Key customization points:

```css
:root {
  --primary-color: #667eea;  /* Change brand colors */
  --secondary-color: #764ba2;
  /* ... more CSS variables */
}
```

### JavaScript

Interactive features are in `public/js/main.js`:
- Mobile menu toggle
- Smooth scrolling
- Scroll animations
- Navbar effects

### Layout

The main layout is in `src/layouts/Layout.astro`. This wraps all pages and includes:
- HTML head with meta tags
- Font imports
- CSS and JS imports

## Directory Structure

```
startup-astro/
├── public/
│   ├── css/
│   │   └── style.css       # Main stylesheet
│   └── js/
│       └── main.js         # JavaScript functionality
├── src/
│   ├── components/
│   │   ├── About.astro     # About section
│   │   ├── CTA.astro       # Call-to-action
│   │   ├── Features.astro  # Features section
│   │   ├── Footer.astro    # Footer
│   │   ├── Hero.astro      # Hero section
│   │   ├── Navbar.astro    # Navigation bar
│   │   └── Testimonials.astro # Testimonials
│   ├── layouts/
│   │   └── Layout.astro    # Main layout wrapper
│   ├── pages/
│   │   └── index.astro     # Homepage
│   └── config.ts           # Site configuration
├── astro.config.mjs        # Astro configuration
├── package.json            # Dependencies and scripts
├── tsconfig.json           # TypeScript configuration
└── README.md              # This file
```

## Astro Features Used

- **Component Islands**: Each section is a reusable component
- **Zero JS by Default**: Minimal JavaScript, only where needed
- **Type Safety**: TypeScript configuration included
- **Static Site Generation**: Pre-renders all pages at build time
- **Fast Refresh**: Instant updates during development

## Performance

- **Minimal JavaScript**: Interactive features only load when needed
- **Optimized CSS**: Pure CSS animations (no heavy libraries)
- **Fast Build Times**: Astro's optimized build process
- **Perfect Lighthouse Scores**: Optimized for Core Web Vitals

## Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Mobile browsers (iOS Safari, Chrome Mobile)

## Tips for Customization

1. **Add Your Logo**: Replace the text logo in `Navbar.astro` with an image
2. **Update Colors**: Modify CSS variables in `public/css/style.css`
3. **Add Real Images**: Replace SVG placeholders with actual product images
4. **Create New Pages**: Add `.astro` files to `src/pages/` directory
5. **Add Analytics**: Include tracking code in `Layout.astro`
6. **Optimize Images**: Use Astro's `<Image />` component for automatic optimization

## Deployment

This Astro site can be deployed to various platforms:

### Vercel
```bash
npm install -g vercel
vercel
```

### Netlify
```bash
npm install -g netlify-cli
netlify deploy
```

### GitHub Pages
Add to `.github/workflows/deploy.yml` and push to GitHub

### Static Hosting
Upload the `dist/` folder to any static hosting provider

## Resources

- [Astro Documentation](https://docs.astro.build)
- [Astro Discord](https://astro.build/chat)
- [Astro Themes](https://astro.build/themes)
- [Astro GitHub](https://github.com/withastro/astro)

## Differences from Hugo Version

This Astro version offers several advantages:
- **Component-Based**: Easier to maintain and reuse components
- **Type Safety**: TypeScript support out of the box
- **Better DX**: Hot module replacement and fast refresh
- **Modern Tooling**: Vite-powered build system
- **Islands Architecture**: Only ship JavaScript where needed
- **Framework Agnostic**: Can integrate React, Vue, Svelte if needed

## License

This example is available under the same license as the Hugo project.

## Credits

Converted from the Hugo startup landing page example to demonstrate Astro's capabilities and modern web development best practices.
