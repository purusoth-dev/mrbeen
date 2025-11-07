# Mr Been Travels - Landing Website

A clean, modern taxi booking website built with Astro and Tailwind CSS. Fast, SEO-friendly, and mobile-first design.

## Features

- **Modern Tech Stack**: Built with Astro (latest) and Tailwind CSS
- **SEO Optimized**: Comprehensive meta tags and semantic HTML
- **Mobile-First Design**: Responsive design optimized for all devices
- **Fast Loading**: Static site generation for optimal performance
- **Interactive Components**:
  - Sticky navigation header
  - Hero section with booking form
  - Services grid
  - Popular tours showcase
  - Transparent pricing tables
  - FAQ accordion
  - Floating action buttons (Call + WhatsApp)
  - Scroll-to-top functionality

## Project Structure

```text
/
├── public/
│   └── favicon.svg
├── src/
│   ├── components/
│   │   ├── Contact.astro
│   │   ├── FAQ.astro
│   │   ├── FloatingButtons.astro
│   │   ├── Footer.astro
│   │   ├── Header.astro
│   │   ├── Hero.astro
│   │   ├── PopularTours.astro
│   │   ├── Pricing.astro
│   │   ├── Services.astro
│   │   └── WhyChooseUs.astro
│   ├── layouts/
│   │   └── Layout.astro
│   ├── pages/
│   │   └── index.astro
│   └── styles/
│       └── global.css
├── astro.config.mjs
├── package.json
├── tailwind.config.mjs
└── tsconfig.json
```

## Getting Started

### Prerequisites

- Node.js 18+
- npm, pnpm, or yarn

### Installation

1. Install dependencies:
```bash
npm install
```

2. Start the development server:
```bash
npm run dev
```

3. Open your browser and visit `http://localhost:4321/`

## Available Commands

| Command | Action |
| :--- | :--- |
| `npm install` | Install dependencies |
| `npm run dev` | Start dev server at `localhost:4321` |
| `npm run build` | Build production site to `./dist/` |
| `npm run preview` | Preview build locally before deploying |

## Customization Guide

### Update Brand Information

Edit the following files to customize your brand:

**Contact Details** - Update in:
- `src/components/Header.astro`
- `src/components/Hero.astro`
- `src/components/Contact.astro`
- `src/components/Footer.astro`
- `src/components/FloatingButtons.astro`

**Services** - Edit `src/components/Services.astro`:
```javascript
const services = [
  {
    icon: "🏙️",
    title: "Your Service",
    description: "Description here",
    features: ["Feature 1", "Feature 2"]
  }
];
```

**Tours & Pricing** - Modify:
- Tours: `src/components/PopularTours.astro`
- Pricing: `src/components/Pricing.astro`

**FAQ** - Update `src/components/FAQ.astro`:
```javascript
const faqs = [
  {
    question: "Your question?",
    answer: "Your answer"
  }
];
```

### Styling

The theme uses a yellow + black color scheme. To customize colors:

**Primary Colors** (used throughout):
- Yellow: `bg-yellow-500`, `text-yellow-500` (Tailwind)
- Black/Gray: `bg-gray-900`, `text-gray-900`

Edit `src/styles/global.css` or component files to change colors.

## Booking Form Behavior

The booking form in `src/components/Hero.astro` currently:
- Opens WhatsApp with pre-filled message
- Includes all form details

To change to alert notification instead:
```javascript
// In Hero.astro <script> section
// Comment out:
// window.open(whatsappUrl, '_blank');

// Uncomment:
// alert("Thanks! We'll contact you shortly.");
```

## SEO

SEO meta tags are configured in `src/layouts/Layout.astro`:
- Title and description
- Open Graph tags
- Twitter Card tags
- Keywords and robots meta

Update these for your specific needs.

## Deployment

### Deploy to Netlify

1. Push to GitHub
2. Connect repository to Netlify
3. Build command: `npm run build`
4. Publish directory: `dist`

### Deploy to Vercel

1. Push to GitHub
2. Import project to Vercel
3. Framework preset: Astro
4. Deploy

### Deploy to Other Platforms

The built static files are in the `./dist/` folder after running:
```bash
npm run build
```

Upload these to any static hosting service.

## Technologies Used

- [Astro](https://astro.build) - Static Site Generator
- [Tailwind CSS](https://tailwindcss.com) - Utility-first CSS framework
- [Heroicons](https://heroicons.com) - SVG icons
- TypeScript - Type safety

## Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Mobile browsers (iOS Safari, Chrome Mobile)

## Performance

- Lighthouse Score: 95+ (Performance, Accessibility, Best Practices, SEO)
- Fast page load times with static generation
- Optimized images and assets
- Minimal JavaScript bundle

## Contact

For support or inquiries:
- Phone: +91 9360615120
- WhatsApp: https://wa.me/919360615120
- Email: info@mrbeentravels.com

## License

This project is private and proprietary.
