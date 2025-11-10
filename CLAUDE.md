# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Mr Been Travels is a taxi booking website built with Astro and TailwindCSS. It's a static site showcasing taxi services in Chennai with sections for services, pricing, contact information, and booking functionality.

## Development Commands

```bash
# Start development server
npm run dev

# Build for production
npm run build

# Preview production build
npm run preview

# Run Astro CLI commands
npm run astro [command]
```

## Architecture

**Framework**: Astro v5 with TypeScript support
**Styling**: TailwindCSS v4 (configured via Vite plugin)
**Structure**: Component-based architecture with layout system

### Directory Structure
- `src/pages/` - Page routes (index.astro is the main landing page)
- `src/layouts/` - Layout components (Layout.astro provides base HTML structure)
- `src/components/` - Reusable Astro components for different page sections
- `src/styles/` - Global CSS (imports TailwindCSS)
- `public/` - Static assets

### Component Architecture
The main page (`index.astro`) imports and renders components in this order:
1. Header (navigation and contact info)
2. Hero (main banner)
3. Services (service offerings)
4. PopularTours (tour packages)
5. Pricing (pricing information)
6. WhyChooseUs (value propositions)
7. FAQ (frequently asked questions)
8. Contact (contact form/info)
9. Footer
10. FloatingButtons (floating action buttons)

### Key Patterns
- Components use Astro's frontmatter syntax with TypeScript
- TailwindCSS classes for styling with yellow branding color (#text-yellow-500)
- Contact information (phone: +91 9363786531) is hardcoded in components
- SEO-optimized with meta tags in Layout.astro
- Responsive design with mobile-first approach

### Configuration
- TypeScript config extends Astro's strict configuration
- TailwindCSS integrated via Vite plugin in astro.config.mjs
- No additional linting, testing, or build tools configured

## Business Context
Mr Been Travels provides taxi services in Chennai for:
- Local rides within city
- Airport pickup/drop services  
- Outstation trips across Tamil Nadu, Pondicherry, Kerala & Andhra Pradesh
- 24x7 service availability