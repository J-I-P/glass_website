# Copilot Instructions for Glass Website

## Project Overview
This is a responsive eyewear/glasses website built as a static site using modern web technologies. The site showcases different collections of glasses, store locations, FAQ, and customer testimonials. It's designed to be deployed on GitHub Pages.

## Technology Stack
- **Build Tool**: Vite (v4.2.0)
- **Templating**: EJS for HTML templating and component reuse
- **Styling**: SCSS/Sass for CSS preprocessing
- **JavaScript**: Vanilla JavaScript (ES modules)
- **Deployment**: GitHub Pages via gh-pages package
- **Package Manager**: npm

## Project Structure
```
/
├── pages/           # Main HTML pages using EJS templates
├── layout/          # Reusable EJS components (header, footer)
├── assets/          # Static assets
│   ├── images/      # Image files
│   └── scss/        # SCSS stylesheets
│       ├── base/    # Base styles, variables, resets
│       ├── layout/  # Layout component styles
│       └── pages/   # Page-specific styles
├── main.js          # Main JavaScript entry point
└── vite.config.js   # Vite configuration
```

## Development Workflow
1. **Setup**: Run `npm install` to install dependencies
2. **Development**: Use `npm run dev` to start development server
3. **Build**: Use `npm run build` to create production build in `/dist`
4. **Deploy**: Use `npm run deploy` to build and deploy to GitHub Pages

## Code Style Guidelines

### HTML/EJS Templates
- Use semantic HTML5 elements
- Include EJS templates with `<%- include('./layout/header'); -%>` syntax
- Maintain consistent indentation (tabs)
- Use descriptive alt text for images
- Follow BEM-like class naming for CSS classes

### SCSS/CSS
- Follow the existing file structure in `/assets/scss/`
- Use SCSS variables defined in `base/_variable.scss`
- Organize styles by component in appropriate directories
- Use responsive design patterns with mobile-first approach
- Media queries are typically at 576px, 768px breakpoints
- Prefer flexbox and CSS Grid for layouts

### JavaScript
- Use ES6+ modules and syntax
- Keep JavaScript minimal and focused on progressive enhancement
- Import/export using ES module syntax
- Main entry point is `main.js`

### Images and Assets
- Store images in `/assets/images/`
- Use descriptive filenames
- Optimize images for web (consider file size)
- Use appropriate image formats (PNG for graphics, JPG for photos)

## Architecture Patterns
- **Component-based**: Reusable layout components in `/layout/`
- **Page-specific**: Individual pages in `/pages/` directory
- **Modular CSS**: SCSS organized by base, layout, and page-specific styles
- **Static Generation**: Vite processes EJS templates into static HTML

## Common Tasks
- **Adding a new page**: Create HTML file in `/pages/`, add corresponding SCSS in `/assets/scss/pages/`
- **Modifying layout**: Edit components in `/layout/` directory
- **Styling changes**: Work in appropriate SCSS files, import in `all.scss`
- **Adding images**: Place in `/assets/images/` and reference with relative paths

## Build Configuration
- Vite is configured to process EJS templates
- SCSS is automatically compiled
- Build output goes to `/dist/` directory
- GitHub Pages deployment is automated via `gh-pages` package

## Browser Support
- Target modern browsers with ES6+ support
- Responsive design for mobile, tablet, and desktop
- Consider accessibility best practices

## Performance Considerations
- Images are major assets, ensure they're optimized
- SCSS compilation should be efficient
- Minimize JavaScript bundle size
- Use Vite's built-in optimizations

## Deployment Notes
- Site is deployed to GitHub Pages
- Base URL is configured as `/glass_website/` in vite.config.js
- Deployment happens via `npm run deploy` command
- Ensure all asset paths are relative and work correctly after build