# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is "Haus Reparaciones" - a business website for a home repair service in Buenos Aires, Argentina. The site is built with Astro and uses Tailwind CSS for styling. It's a static site showcasing repair services (albañilería, plomería, pintura, Durlock), service details, and contact information.

## Development Commands

All commands run from the project root:

- `npm install` - Install dependencies
- `npm run dev` - Start development server at localhost:4321
- `npm run build` - Build production site to ./dist/
- `npm run preview` - Preview production build locally
- `npm run astro ...` - Run Astro CLI commands

## Architecture

### Tech Stack
- **Astro 5.10.1**: Static site generator with component-based architecture
- **Tailwind CSS 4.1.11**: Utility-first CSS framework via Vite plugin
- **TypeScript**: Strict configuration extending astro/tsconfigs/strict
- **FontAwesome 6.7.2**: Icon library

### Project Structure
- `src/layouts/`: Base layout components (BaseLayout.astro provides main structure)
- `src/components/`: Reusable components (Header.astro, Footer.astro)
- `src/pages/`: Route-based pages (index, about, contact, etc.)
- `src/styles/`: Global styles (tailwind.css imports)
- `public/images/`: Customer testimonial screenshots
- `astro.config.mjs`: Includes ngrok configuration for development tunneling

### Key Features
- Spanish-language business site for home repair services
- Services showcase with grid layout for albañilería, plomería, pintura, and Durlock
- Detailed service descriptions and contact forms
- SSL certificate setup documented for hausreparaciones.com domain
- Responsive design with Tailwind CSS

### Development Notes
- Uses Vite with Tailwind CSS plugin integration
- Configured for ngrok tunneling (allowedHosts setting)
- Images stored in public/images/ for customer testimonials
- ESM modules available via esm.sh for client-side functionality