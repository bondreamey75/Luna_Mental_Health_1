# Luna - Mental Wellness Application

## Overview

Luna is a comprehensive mental wellness and emotional support web application built with modern technologies. The application provides users with tools for emotional tracking, daily check-ins, journaling, and data insights to support their mental health journey.

## Project Structure

```
website-code/
├── client/                    # Frontend React application
│   ├── src/
│   │   ├── components/        # Reusable UI components
│   │   │   └── ui/           # shadcn/ui components
│   │   ├── contexts/         # React contexts (Theme)
│   │   ├── hooks/            # Custom React hooks
│   │   ├── lib/              # Utility libraries (queryClient, utils)
│   │   ├── pages/            # Application pages/routes
│   │   ├── App.tsx           # Main app component with routing
│   │   ├── main.tsx          # React entry point
│   │   └── index.css         # Global styles and CSS variables
│   └── index.html            # HTML template
├── server/                   # Backend Express.js application
│   ├── db.ts                # Database configuration
│   ├── index.ts             # Server entry point
│   ├── routes.ts            # API routes
│   ├── storage.ts           # Data storage interface
│   └── vite.ts              # Vite integration for development
├── shared/                  # Shared code between client and server
│   └── schema.ts            # Database schema and types
├── package.json             # Project dependencies and scripts
├── vite.config.ts           # Vite build configuration
├── tailwind.config.ts       # Tailwind CSS configuration
├── tsconfig.json            # TypeScript configuration
├── drizzle.config.ts        # Drizzle ORM configuration
├── postcss.config.js        # PostCSS configuration
└── components.json          # shadcn/ui configuration
```

## Technology Stack

### Frontend
- **React 18** - UI library with hooks and modern patterns
- **TypeScript** - Type safety and enhanced developer experience
- **Vite** - Fast build tool and development server
- **Wouter** - Lightweight client-side routing
- **TanStack Query** - Server state management and data fetching
- **Tailwind CSS** - Utility-first CSS framework
- **shadcn/ui** - Accessible and customizable UI components built on Radix UI
- **Framer Motion** - Animation library
- **Lucide React** - Icon library

### Backend
- **Express.js** - Web application framework
- **TypeScript** - Type safety for server-side code
- **Drizzle ORM** - Type-safe database ORM
- **PostgreSQL** - Primary database (via Neon serverless)
- **Zod** - Schema validation

### Development Tools
- **ESBuild** - Fast JavaScript bundler for server builds
- **Drizzle Kit** - Database schema management and migrations
- **PostCSS** - CSS processing
- **Autoprefixer** - CSS vendor prefixes

## Pages and Features

1. **Home** (`/`) - Landing page with navigation cards to all features
2. **Data Insights** (`/data-insights`) - Visualizations and analytics
3. **Daily Check-in** (`/daily-checkin`) - Mood tracking and daily reflections
4. **Explore** (`/explore`) - Wellness resources and techniques
5. **Luna ChatBot** (`/luna-chatbot`) - AI-powered emotional support assistant
6. **Journaling** (`/journaling`) - Personal journaling interface

## Styling and Design

- **Design System**: Custom purple/pink gradient color scheme optimized for wellness applications
- **Dark Mode**: Full dark mode support with automatic theme switching
- **Glassmorphism**: Modern glass-like UI effects with backdrop blur
- **Responsive Design**: Mobile-first approach with responsive layouts
- **Animations**: Smooth transitions and floating animations for enhanced UX

## Getting Started

### Prerequisites
- Node.js 18+ 
- npm or yarn
- PostgreSQL database

### Installation

1. Install dependencies:
```bash
npm install
```

2. Set up environment variables:
Create a `.env` file with:
```
DATABASE_URL=your_postgresql_connection_string
```

3. Set up the database:
```bash
npm run db:push
```

4. Start the development server:
```bash
npm run dev
```

The application will be available at `http://localhost:5000`

### Build for Production

```bash
npm run build
npm start
```

## Scripts

- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm run start` - Start production server
- `npm run check` - Run TypeScript type checking
- `npm run db:push` - Push database schema changes

## Database Schema

The application uses PostgreSQL with the following main tables:
- **users** - User accounts and authentication
- **journal_entries** - Personal journal entries with timestamps

## Architecture Highlights

- **Full-stack TypeScript** for type safety across client and server
- **Modern React patterns** with hooks, contexts, and custom hooks
- **Component-based architecture** with reusable UI components
- **RESTful API design** with Express.js routes
- **Type-safe database operations** with Drizzle ORM
- **Responsive and accessible design** with shadcn/ui components
- **Optimized development experience** with hot reload and TypeScript integration

## Authors

Created by Vedant Gophane, Arya Yadav, Kaivalya Lehekar, Chirashree Bapuli and Amey Bondre