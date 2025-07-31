# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is Drew "Dr.C" Clinkenbeard's personal academic website built using Jekyll with the al-folio theme. The site is hosted on GitHub Pages and serves as a portfolio, blog, and academic presence at https://clinkenbeard.info.

## Architecture

**Jekyll Static Site Generator**: The site uses Jekyll with Ruby gems for static site generation.

**al-folio Theme**: Built on the al-folio academic theme with extensive customization for personal use.

**Content Structure**:
- `_posts/` - Blog posts (markdown with front matter)
- `_projects/` - Project showcases 
- `_books/` - Book reviews and reading list
- `_pages/` - Static pages (about, CV, publications, etc.)
- `_data/` - YAML data files (CV info, social links, etc.)
- `_includes/` - Reusable template partials
- `_layouts/` - Page layout templates
- `_sass/` - Styling and theme customization

**Key Features**:
- Responsive design with light/dark mode
- Academic publications with Jekyll Scholar
- Image optimization via ImageMagick
- Mathematical typesetting with MathJax
- Search functionality
- Multi-format content support (videos, audio, interactive elements)

## Common Development Commands

### Building and Serving
```bash
# Install dependencies
bundle install
npm install

# Serve development site with live reload
bundle exec jekyll serve --livereload

# Build for production
bundle exec jekyll build

# Format code 
npx prettier --write . --ignore-path .gitignore
```

### Content Creation
- Blog posts go in `_posts/` with naming: `YYYY-MM-DD-title.md`
- Projects go in `_projects/` 
- Book reviews go in `_books/`
- Update CV data in `_data/cv.yml`

### Image Handling
ImageMagick is required and configured to generate responsive images in multiple formats (WebP). Images should be placed in `assets/img/` and will be automatically optimized during build.

## Configuration Notes

**Jekyll Configuration**: Primary config in `_config.yml` with extensive customization for academic features, social links, and theme options.

**Dependencies**: 
- Ruby gems managed via Gemfile (Jekyll plugins and themes)
- Node packages for Prettier formatting and Puppeteer
- ImageMagick for image processing

**Deployment**: Automated via GitHub Pages, builds automatically on push to main branch.

## Development Workflow

1. Create content in appropriate `_posts/`, `_projects/`, or `_pages/` directories
2. Test locally with `bundle exec jekyll serve --livereload`
3. Format code with Prettier before committing
4. Push to GitHub for automatic deployment

The site architecture follows Jekyll conventions with the al-folio theme's extended academic features for publications, CV management, and rich content display.