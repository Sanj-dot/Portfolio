# Sanjida A. Portfolio Website

## Overview

This is a professional portfolio website built for Sanjida A., a government and finance professional with expertise in digital transformation, taxation reform, and public sector efficiency. The application is a full-stack web application with a React frontend and Express backend, featuring an elegant emerald/teal color scheme, Garamond typography, professional logo design, and smooth animations with a fully functional contact form system.

## User Preferences

Preferred communication style: Simple, everyday language.
Design preferences: Modern Slate Blue & Lavender color scheme with Inter fonts for clean, readable typography. Limited to 2-3 main colors with lots of white space for a clean, professional look.

## System Architecture

### Frontend Architecture
- **Framework**: React 18 with TypeScript
- **Build Tool**: Vite for fast development and optimized builds
- **Styling**: Tailwind CSS with custom CSS variables for theming
- **UI Components**: Radix UI primitives with custom shadcn/ui components
- **Animations**: Framer Motion for smooth page transitions and animations
- **Routing**: Wouter for lightweight client-side routing
- **State Management**: React Query (TanStack Query) for server state management
- **Form Handling**: React Hook Form with Zod validation

### Backend Architecture
- **Framework**: Express.js with TypeScript
- **Database**: PostgreSQL with Drizzle ORM
- **Database Provider**: Neon Database (serverless PostgreSQL)
- **Development**: Hot reloading with Vite integration
- **Session Management**: PostgreSQL session store with connect-pg-simple
- **API Design**: RESTful API with JSON responses

## Key Components

### Frontend Components
- **Navigation**: Fixed header with smooth scroll navigation
- **Hero Section**: Animated landing area with call-to-action buttons
- **About Section**: Professional summary with contact information
- **Experience Timeline**: Interactive timeline of professional experience
- **Skills Section**: Technical and professional competencies display
- **Expertise Section**: Detailed breakdown of professional areas
- **Podcast Section**: Showcases "Policy Charcha" podcast with Spotify integration
- **Articles Section**: Placeholder for upcoming articles and thought leadership content
- **Contact Section**: Form with validation and submission handling
- **Footer**: Social links including LinkedIn and Spotify podcast links

### Backend Components
- **Storage Layer**: Abstracted storage interface with in-memory fallback
- **API Routes**: Contact form submission and admin endpoints
- **Database Schema**: User and contact submission tables
- **Error Handling**: Centralized error handling middleware
- **Development Tools**: Request logging and response timing

## Data Flow

1. **Contact Form Submission**:
   - User fills out contact form with validation
   - Form data is validated using Zod schema
   - React Query handles API request to backend
   - Express validates and stores submission in database
   - Success/error feedback displayed via toast notifications

2. **Static Content**:
   - Portfolio content is statically defined in components
   - No dynamic content loading from backend for portfolio sections
   - All professional information is hardcoded in React components

3. **Admin Access**:
   - Backend provides endpoint to retrieve all contact submissions
   - Currently no authentication system implemented

## External Dependencies

### Frontend Dependencies
- **@radix-ui/***: Comprehensive UI primitive components
- **@tanstack/react-query**: Server state management
- **framer-motion**: Animation library
- **react-hook-form**: Form handling
- **@hookform/resolvers**: Form validation resolvers
- **zod**: Schema validation
- **tailwindcss**: Utility-first CSS framework
- **wouter**: Lightweight routing

### Backend Dependencies
- **express**: Web application framework
- **drizzle-orm**: Type-safe ORM
- **@neondatabase/serverless**: Neon database driver
- **connect-pg-simple**: PostgreSQL session store
- **tsx**: TypeScript execution for development

### Development Dependencies
- **vite**: Build tool and development server
- **@vitejs/plugin-react**: React support for Vite
- **drizzle-kit**: Database migrations and tooling
- **@replit/vite-plugin-runtime-error-modal**: Development error handling
- **@replit/vite-plugin-cartographer**: Replit integration

## Deployment Strategy

### Development Environment
- **Dev Server**: Vite development server with hot reloading
- **Database**: Neon serverless PostgreSQL
- **Environment**: Node.js with tsx for TypeScript execution
- **Build Process**: Vite for frontend, esbuild for backend

### Production Build
- **Frontend**: Vite builds React app to `dist/public`
- **Backend**: esbuild bundles Express server to `dist/index.js`
- **Static Assets**: Served directly by Express in production
- **Database**: PostgreSQL via Neon with connection pooling

### Configuration
- **TypeScript**: Shared configuration for frontend, backend, and shared code
- **Path Aliases**: Configured for clean imports (`@/`, `@shared/`)
- **Environment Variables**: `DATABASE_URL` required for database connection
- **Port Configuration**: Express server runs on configurable port

### Database Management
- **Migrations**: Drizzle Kit handles schema migrations
- **Schema**: Centralized in `shared/schema.ts`
- **Development**: Push schema changes with `npm run db:push`
- **Production**: Migration files generated in `./migrations` directory

The application follows a monorepo structure with clear separation between client, server, and shared code, making it maintainable and scalable for future enhancements.

## Recent Changes

### Design Transformation (July 16, 2025)
- **Color Scheme**: Transitioned from emerald/teal to modern Slate Blue & Lavender palette
  - Primary: Slate Blue for headers, highlights, and navigation
  - Accent: Lavender for buttons, links, and interactive elements
  - Background: Clean light shades with lots of white space
- **Typography**: Migrated from EB Garamond to Inter font for modern, readable appearance
  - Applied Inter font family across all components and UI elements
  - Enhanced readability and contemporary professional look
- **Logo Updates**: Updated gradient colors to match new Slate Blue & Lavender theme
- **Background Updates**: Refreshed all gradient backgrounds to align with new color palette
- **Clean Design**: Implemented 2-3 main colors approach with extensive white space
- **Status**: Color scheme and typography transformation completed successfully