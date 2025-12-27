# next-fsd

Production-ready base project for building Next.js applications
with App Router and strict Feature-Sliced Design architecture.

This repository provides a preconfigured foundation focused on
scalability, architectural consistency, and developer experience.

## Purpose

`next-fsd` is a base project intended to be used as:

- a starting point for new Next.js applications
- a reference implementation of Feature-Sliced Design with App Router
- an internal company template for frontend projects
- a foundation for scalable, long-living React/Next.js codebases

## Requirements

- Node.js >= 24
- npm >= 11

## What's included

### Next.js

- Next.js with App Router
- React Server Components support
- TypeScript strict mode
- CSS Modules and Sass support

### Feature-Sliced Design

- Strict layer-based architecture:
  - `app`
  - `pages`
  - `widgets`
  - `features`
  - `entities`
  - `shared`
- Clear separation of responsibility by layers and segments
- Predictable project structure for large teams

## Architecture enforcement (FSD)

The project uses ESLint boundaries rules to enforce Feature-Sliced Design
layer dependencies at lint time, preventing invalid imports between layers.

### ESLint (architecture-aware)

- ESLint 9 (flat config)
- `eslint-config-next` (core-web-vitals)
- Architectural rules enforced via `eslint-plugin-boundaries`
- Layer dependency control (FSD rules)
- Sorted imports (`eslint-plugin-simple-import-sort`)
- Integrated Prettier compatibility

### Code quality

- Prettier integration
- Consistent formatting and linting rules
- Ready for CI usage

### Testing

- Jest
- React Testing Library
- jsdom environment
- Ready for component and unit testing

### CI

- GitLab CI configuration
- Lint and test stages out of the box

## Non-goals

This repository does NOT try to:

- provide UI components or design system
- solve state management choices for you
- include authentication or API logic
- abstract Next.js or hide framework details

The goal is to provide a clean, minimal, and opinionated foundation,
not a feature-complete application.

## Who is this for

This project is intended for:

- frontend engineers building scalable Next.js applications
- teams adopting Feature-Sliced Design
- developers who want strict architectural guarantees
- companies needing a stable internal frontend template

## Getting started

```bash
git clone https://github.com/SlavaSlimmy/next-fsd.git
cd next-fsd
npm install
npm run dev
```

---

## Tech stack

- Next.js
- React
- TypeScript
- ESLint 9
- Prettier
- Jest
- Sass

## License

MIT
