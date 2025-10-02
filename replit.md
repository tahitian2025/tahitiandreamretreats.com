# Replit.md

## Overview

Tahitian Dream Retreats is a luxury pool design and construction company website built as a modern React single-page application. The site showcases premium pool services including custom design, new construction, remodeling, and home additions. It features a sophisticated design system with luxury branding, interactive components, and a contact form for lead generation.

## User Preferences

Preferred communication style: Simple, everyday language.

## System Architecture

### Frontend Architecture
- **Framework**: React 18 with TypeScript, using Vite as the build tool
- **Routing**: Wouter for lightweight client-side routing
- **State Management**: TanStack Query for server state management
- **UI Framework**: shadcn/ui component library with Radix UI primitives
- **Styling**: Tailwind CSS with custom design tokens matching luxury brand guidelines
- **Typography**: Inter/Poppins for body text, Playfair Display for headings

### Design System
- **Color Palette**: Deep teal primary, sunset orange accent, warm gold highlights
- **Component Library**: Comprehensive UI components following luxury hospitality design patterns
- **Layout System**: Tailwind spacing units (4, 8, 12, 16, 24) with generous whitespace
- **Responsive Design**: Mobile-first approach with breakpoint-specific layouts

### Backend Architecture
- **Runtime**: Node.js with Express.js server
- **Database ORM**: Drizzle ORM with PostgreSQL dialect
- **API Design**: RESTful endpoints for contact form submissions
- **Data Storage**: In-memory storage implementation with interface for database migration
- **Session Management**: Prepared for connect-pg-simple session store

### Data Layer
- **Schema**: Contact submissions table with form data (name, email, phone, service type, budget, message)
- **Validation**: Zod schemas for runtime type checking and data validation
- **Database**: PostgreSQL with Drizzle migrations (configured for Neon serverless)

### Development Tools
- **TypeScript**: Strict type checking across client and server
- **Build Process**: Vite for frontend, esbuild for server bundling
- **Hot Reload**: Vite development server with HMR
- **Path Aliases**: Configured for clean imports (@/, @shared/, @assets/)

## External Dependencies

### Database Services
- **Neon Database**: Serverless PostgreSQL hosting
- **Drizzle Kit**: Database migrations and schema management

### UI and Styling
- **Radix UI**: Headless component primitives for accessibility
- **Tailwind CSS**: Utility-first CSS framework
- **Lucide React**: Icon library for consistent iconography
- **Google Fonts**: Inter, Poppins, and Playfair Display typography

### Development Dependencies
- **Vite**: Frontend build tool and development server
- **ESBuild**: Fast JavaScript bundler for server builds
- **PostCSS**: CSS processing with Tailwind and Autoprefixer

### Form and Validation
- **React Hook Form**: Form state management with performance optimization
- **Hookform Resolvers**: Integration with Zod validation schemas
- **Zod**: Runtime type validation and schema definition

### Assets and Media
- **Generated Images**: AI-generated luxury pool imagery stored in attached_assets
- **Logo Assets**: Custom Tahitian Dream Retreats branding with sunset and heron design
- **Portfolio Images**: 8 real luxury pool project photos showcasing company work

## Recent Changes

### October 2, 2025
- **SEO Implementation**: Added comprehensive SEO with react-helmet-async across all 7 pages
  - Unique meta tags, Open Graph tags, Twitter Cards for each page
  - JSON-LD structured data (LocalBusiness, Service, Organization schemas)
  - sitemap.xml and robots.txt for search engine crawling
- **Service Area Optimization**: Reduced from 39 to 25 premium Houston areas
  - Focused on affluent neighborhoods: River Oaks, Memorial, Tanglewood, Piney Point Village, Bunker Hill Village
  - Added luxury suburbs: Cinco Ranch, Sienna Plantation, Hunter's Creek Village, Hedwig Village
  - Removed less relevant areas: Downtown Houston, Gulfton, Pasadena, Greenway Plaza, etc.
  - Updated Contact and Footer components with optimized service areas

### October 1, 2025
- **New Dedicated Pages**: 
  - Pavilions & Pergolas (/pavilions-pergolas): 5 design styles, luxury add-ons, scalable options
  - Outdoor Kitchens (/outdoor-kitchens): 4 kitchen types (basic to luxury), design enhancements, material themes
  - Home Additions (/home-additions): 7 addition categories from lifestyle expansions to poolside structures
- **Services Page Enhancement**: Added "Learn More" buttons to Pavilions & Pergolas, Outdoor Kitchens, and Home Additions service cards
- **Portfolio Cleanup**: Removed portfolio items with mountain/landscape backgrounds

### September 22, 2025
- **Pages Added**: About Us (/about), Services (/services), FAQ (/faq), Contact (/contact)
- **Technical Improvements**: Navigation fixes, router updates, form integration, responsive design
- **Content Structure**: Professional copy, service offerings, Houston geographic focus, lead generation touchpoints