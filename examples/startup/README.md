# Startup Landing Page - Hugo Example

A modern, responsive landing page template for startups built with Hugo static site generator.

## Features

- **Modern Design**: Clean, professional design with gradient accents
- **Fully Responsive**: Mobile-first design that looks great on all devices
- **Smooth Animations**: Scroll animations and hover effects
- **SEO Friendly**: Semantic HTML with proper meta tags
- **Fast Loading**: Minimal dependencies, optimized CSS
- **Easy to Customize**: Well-organized code and clear structure

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

- Hugo static site generator installed
- Basic knowledge of Hugo and Markdown

### Installation

1. Navigate to this directory:
   ```bash
   cd examples/startup
   ```

2. Run Hugo development server:
   ```bash
   hugo server -D
   ```

3. Open your browser and visit:
   ```
   http://localhost:1313
   ```

### Building for Production

To build the static site for deployment:

```bash
hugo
```

The generated site will be in the `public/` directory.

## Customization

### Update Site Configuration

Edit `config.toml` to customize:
- Site title and description
- Company name and tagline
- Contact information
- Social media links

```toml
[params]
  company_name = "YourCompany"
  tagline = "Your Custom Tagline"
  email = "hello@yourcompany.com"
  # ... more settings
```

### Modify Content

Edit `content/_index.md` to change the main content:

```markdown
---
title: "Your Custom Title"
description: "Your description"
---

# Your content here
```

### Customize Sections

All sections are modular partials in `layouts/partials/`:
- `hero.html` - Hero section
- `features.html` - Features grid
- `about.html` - About section
- `testimonials.html` - Customer testimonials
- `cta.html` - Call-to-action
- `footer.html` - Footer

Edit any partial to customize its content and structure.

### Styling

The main stylesheet is in `static/css/style.css`. Key customization points:

```css
:root {
  --primary-color: #667eea;  /* Change brand colors */
  --secondary-color: #764ba2;
  /* ... more CSS variables */
}
```

### JavaScript

Interactive features are in `static/js/main.js`:
- Mobile menu toggle
- Smooth scrolling
- Scroll animations
- Navbar effects

## Directory Structure

```
startup/
├── config.toml              # Site configuration
├── content/
│   └── _index.md           # Homepage content
├── layouts/
│   ├── index.html          # Main homepage layout
│   └── partials/
│       ├── head.html       # HTML head section
│       ├── navbar.html     # Navigation bar
│       ├── hero.html       # Hero section
│       ├── features.html   # Features section
│       ├── about.html      # About section
│       ├── testimonials.html # Testimonials
│       ├── cta.html        # Call-to-action
│       └── footer.html     # Footer
└── static/
    ├── css/
    │   └── style.css       # Main stylesheet
    ├── js/
    │   └── main.js         # JavaScript functionality
    └── img/                # Images directory
```

## Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Mobile browsers (iOS Safari, Chrome Mobile)

## Tips for Customization

1. **Add Your Logo**: Replace the text logo in `navbar.html` with an image
2. **Update Colors**: Modify CSS variables in `style.css`
3. **Add Real Images**: Replace SVG placeholders with actual product images
4. **Extend Sections**: Add new partial templates for additional sections
5. **Add Analytics**: Include tracking code in `head.html`

## Performance

- Minimal JavaScript (< 2KB)
- Pure CSS animations (no jQuery)
- Optimized for Core Web Vitals
- Fast page load times

## License

This example is part of the Hugo project and is available under the same license as Hugo.

## Resources

- [Hugo Documentation](https://gohugo.io/documentation/)
- [Hugo Themes](https://themes.gohugo.io/)
- [Hugo Discourse](https://discourse.gohugo.io/)

## Credits

Created as an example for the Hugo static site generator to demonstrate modern landing page best practices.
