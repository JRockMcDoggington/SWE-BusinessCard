# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Build & Development Commands

- `npm run dev` — Start development server with hot reload
- `npm run build` — Production build
- `npm run start` — Start production server
- `npm run lint` — Run ESLint

## Tech Stack

- **Next.js 16** with App Router (`app/` directory)
- **React 19** with TypeScript (strict mode)
- **Tailwind CSS v4** via PostCSS plugin (`@tailwindcss/postcss`)
- **Geist font family** (sans & mono) via `next/font`

## Architecture

- App Router: all routes live under `app/`, server components by default
- Path alias `@/*` maps to the project root
- Theming uses CSS custom properties in `app/globals.css` with light/dark mode via `prefers-color-scheme`
- Tailwind v4 theme customization is done inline in `globals.css` using `@theme`
