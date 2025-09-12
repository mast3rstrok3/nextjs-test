# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a Next.js 15.5.3 application using the App Router architecture with TypeScript, React 19, and Tailwind CSS v4.

## Development Commands

```bash
# Start development server with Turbopack
npm run dev

# Build for production with Turbopack
npm run build

# Start production server
npm run start

# Run ESLint
npm run lint
```

## Architecture

### App Router Structure
- `/app` directory contains the application routes and components
- `layout.tsx` - Root layout with Geist font configuration
- `page.tsx` - Page components for each route
- `globals.css` - Global styles with Tailwind CSS directives

### Key Technologies
- **Next.js 15.5.3** with App Router and Turbopack enabled
- **React 19.1.0** and React DOM 19.1.0
- **TypeScript** with strict mode enabled
- **Tailwind CSS v4** using PostCSS plugin architecture (`@tailwindcss/postcss`)
- **ESLint** with Next.js core-web-vitals and TypeScript configurations

### Configuration Files
- `next.config.ts` - Next.js configuration (currently minimal)
- `tsconfig.json` - TypeScript configuration with path alias `@/*` mapping to root
- `eslint.config.mjs` - ESLint flat config using FlatCompat for Next.js rules
- `postcss.config.mjs` - PostCSS with Tailwind CSS plugin

## Development Notes

- The project uses Turbopack for both development and production builds for faster compilation
- Path imports use the `@/` alias which maps to the project root
- ESLint is configured to ignore `node_modules`, `.next`, `out`, `build`, and `next-env.d.ts`
- Tailwind CSS v4 is configured using the new PostCSS plugin approach rather than a traditional config file