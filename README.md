# Sanjida A. - Professional Portfolio

A modern, privacy-focused portfolio website built for Sanjida A., a government and finance professional specializing in digital transformation, policy analysis, and public sector efficiency.

## 🚀 Live Demo

[Visit Portfolio](https://your-portfolio-url.replit.app)

> **Status**: ✅ Application is fully functional and ready for deployment
> - Database connectivity verified
> - Contact form working correctly
> - All API endpoints tested and operational

## 📋 Features

### Core Functionality
- **Privacy-Focused Design**: No phone number display, project details available via email inquiry
- **Interactive Contact Form**: Database-integrated contact system for professional inquiries
- **Professional Showcase**: Comprehensive display of skills, experience, and expertise
- **Responsive Design**: Optimized for all devices with smooth animations

### Technical Features
- **Modern Stack**: React 18 + TypeScript + Express.js + PostgreSQL
- **Real-time Database**: Contact form submissions stored in PostgreSQL
- **Smooth Animations**: Framer Motion for professional user experience
- **Glass Morphism UI**: Modern design with gradient backgrounds
- **SEO Optimized**: Structured data and meta tags for better visibility

### Professional Sections
- **Hero Section**: Professional introduction with call-to-action
- **About**: Detailed professional summary and achievements
- **Experience Timeline**: Interactive career progression display
- **Skills**: Technical expertise and professional competencies
- **Expertise Areas**: Specialized knowledge domains including:
  - Government Digital Transformation
  - Policy Analysis & Drafting
  - Data Analysis & Dashboards
  - Business Development
  - Finance Management
  - Digital Integration
- **Podcast Integration**: "Policy Charcha" podcast with Spotify links
- **Articles Section**: Ready for future content additions
- **Contact Form**: Professional inquiry system with database storage

## 🛠️ Tech Stack

### Frontend
- **React 18** with TypeScript
- **Vite** for build tooling
- **Tailwind CSS** for styling
- **Framer Motion** for animations
- **Radix UI** components with shadcn/ui
- **React Query** for state management
- **React Hook Form** with Zod validation
- **Wouter** for routing

### Backend
- **Express.js** with TypeScript
- **PostgreSQL** with Drizzle ORM
- **Neon Database** (serverless PostgreSQL)
- **Session Management** with PostgreSQL store

### Key Libraries
- `@tanstack/react-query` - Server state management
- `framer-motion` - Animations and transitions
- `drizzle-orm` - Type-safe database operations
- `zod` - Schema validation
- `react-hook-form` - Form handling
- `lucide-react` - Icons
- `tailwindcss` - Utility-first CSS

## 📁 Project Structure

```
├── client/                 # React frontend
│   ├── src/
│   │   ├── components/     # Reusable UI components
│   │   │   ├── ui/        # shadcn/ui components
│   │   │   ├── hero-section.tsx
│   │   │   ├── about-section.tsx
│   │   │   ├── experience-timeline.tsx
│   │   │   ├── skills-section.tsx
│   │   │   ├── expertise-section.tsx
│   │   │   ├── podcast-section.tsx
│   │   │   ├── contact-section.tsx
│   │   │   └── footer.tsx
│   │   ├── pages/         # Page components
│   │   ├── hooks/         # Custom React hooks
│   │   ├── lib/           # Utility functions
│   │   └── main.tsx       # App entry point
│   └── index.html
├── server/                 # Express backend
│   ├── db.ts              # Database connection
│   ├── storage.ts         # Data layer abstraction
│   ├── routes.ts          # API routes
│   └── index.ts           # Server entry point
├── shared/                 # Shared types and schemas
│   └── schema.ts          # Database schema and types
├── package.json
├── vite.config.ts
├── tailwind.config.ts
└── drizzle.config.ts
```

## 🚀 Getting Started

### Prerequisites
- Node.js (v18 or higher)
- PostgreSQL database

### Installation

1. Clone the repository:
```bash
git clone https://github.com/Sanj-dot/Portfolio.git
cd Portfolio
```

2. Install dependencies:
```bash
npm install
```

3. Set up environment variables:
```bash
# Create .env file with:
DATABASE_URL=your_postgresql_connection_string
```

4. Initialize database:
```bash
npm run db:push
```

5. Start development server:
```bash
npm run dev
```

## 💾 Database Schema

The application uses PostgreSQL with the following tables:

### Users Table
- `id` (Primary Key)
- `username` (Unique)
- `password`

### Contact Submissions Table
- `id` (Primary Key)
- `name`
- `email`
- `message`
- `created_at`

## 🎨 Design Philosophy

### Privacy-First Approach
- No personal phone number display
- Project details accessible only through professional inquiry
- Secure contact form with database storage
- Professional networking focus

### Modern UI/UX
- Glass morphism effects with gradient backgrounds
- Smooth scroll navigation
- Interactive timeline components
- Responsive grid layouts
- Professional color scheme

### Performance Optimized
- Lazy loading for images
- Optimized animations
- Efficient database queries
- Fast build times with Vite

## 📄 API Endpoints

### Contact Form
- `POST /api/contact` - Submit contact form
- `GET /api/contact-submissions` - Get all submissions (admin)

### User Management
- `POST /api/register` - User registration
- `POST /api/login` - User authentication

## 🔧 Development Scripts

```bash
npm run dev          # Start development server
npm run build        # Build for production
npm run preview      # Preview production build
npm run db:push      # Push database schema changes
npm run db:generate  # Generate migration files
```

## 🌐 Deployment

### Replit Deployment
1. Click "Deploy" in Replit interface
2. Choose "Autoscale Deployment"
3. Configure settings and deploy

### Manual Deployment
1. Build the application: `npm run build`
2. Set up PostgreSQL database
3. Configure environment variables
4. Deploy to your hosting platform

## 🤝 Professional Contact

For professional inquiries, business collaboration, or project discussions, please use the contact form on the website. All submissions are securely stored and reviewed promptly.

## 📜 License

This project is proprietary and confidential. All rights reserved.

---

Built with ❤️ for professional excellence in government and finance sector transformation.