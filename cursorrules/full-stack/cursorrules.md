You are an expert in React, Supabase, and Tailwind CSS. You follow modern best practices and patterns for full-stack web development.

# Code Style and Structure

- Write clean, maintainable JavaScript/TypeScript with clear examples
- Use functional programming patterns; avoid classes
- Implement modular architecture with clear separation of concerns
- Use descriptive variable names (e.g., isLoading, hasError)
- Structure files consistently: components, utilities, database queries, API routes

# Project Organization

- Organize source code under /src directory
- Create feature-based folders for components and functionality
- Structure the project following Vite + Netlify conventions:

  ```
  /
  ├── /src
  │   ├── /components
  │   │   ├── /ui
  │   │   ├── /forms
  │   │   └── /layouts
  │   ├── /features
  │   │   └── /(feature-specific-folders)
  │   ├── /lib
  │   │   ├── /utils
  │   │   └── /supabase
  │   ├── /routes
  │   │   └── /(route-components)
  │   ├── /types
  │   ├── /assets
  │   ├── App.tsx
  │   └── main.tsx
  ├── /netlify
  │   └── /functions
  │       ├── /api
  │       └── /(serverless-functions)
  ├── /public
  ├── index.html
  ├── vite.config.ts
  └── netlify.toml
  ```

- Serverless functions handle secure database operations
- Client-side Supabase interactions are limited to authenticated operations
- Backend logic lives in the `/netlify/functions` directory
- Frontend utilities and configurations remain in `/lib`

# Frontend Development

## Components

- Use shadcn/ui components as the primary UI component library
- Customize and extend shadcn/ui components using the CLI
- Follow shadcn/ui's component architecture and styling patterns
- Keep components focused and single-purpose
- Implement proper error boundaries
- Place reusable component hooks in separate files
- Structure component folders with index.tsx, types.ts, and hooks.ts

## UI Library Usage

### shadcn/ui Components

- Use shadcn/ui's pre-built components for consistent UI elements
- Leverage the shadcn/ui CLI to add and customize components
- Follow the registry pattern for component organization
- Maintain consistent keyboard navigation patterns
- Follow WAI-ARIA patterns provided by components
- Create consistent component APIs across the application

### Component Organization

```
/src/components
├── /ui
│   ├── /button
│   │   ├── index.tsx
│   │   └── variants.ts
│   ├── /dialog
│   │   ├── index.tsx
│   │   └── hooks.ts
│   └── /...
├── /forms
│   ├── /select
│   ├── /input
│   └── /...
└── /layouts
    ├── /header
    ├── /footer
    └── /...
```

## Tailwind CSS

- Create consistent component styles using Tailwind composition
- Use classes={clsx()} for conditional styling
- Create reusable utility classes in components/ui/styles.ts
- Follow mobile-first responsive design
- Maintain a consistent color palette
- Use CSS variables for theme values
- Implement dark mode using Tailwind's dark: modifier
- Create reusable patterns with @apply in component-specific CSS files when needed

# Performance and Optimization

- Implement proper caching strategies
- Use proper image optimization
- Implement code splitting
- Monitor and optimize Core Web Vitals
- Use proper SEO practices

# Security

- Implement proper authentication
- Use proper CORS policies
- Validate all user input
- Follow security best practices

# Testing

- Write unit tests for utilities
- Implement integration tests
- Use proper testing libraries
- Follow testing best practices
- Maintain good test coverage

# Development Workflow

- Use proper Git workflow
- Implement proper CI/CD
- Follow conventional commits
- Use proper linting and formatting
- Implement proper documentation

# Error Handling

- Implement proper error boundaries
- Use consistent error messages
- Implement proper logging
- Handle edge cases appropriately
- Provide meaningful user feedback

# State Management

- Use React Query for server state
- Implement proper local state management
- Use proper caching strategies
- Follow proper data flow patterns
- Implement proper loading states

```

```
