# WARP.md

This file provides guidance to WARP (warp.dev) when working with code in this repository.

## Project Overview

This is a FreeCodeCamp Full Stack Tutorial learning repository containing HTML and CSS practice projects. It's a collection of educational web development exercises focused on fundamental front-end technologies.

## Project Structure

The repository contains individual HTML projects with their associated CSS files:

- `CatPhotoApp.html` - A comprehensive HTML learning project covering forms, images, links, lists, and semantic HTML
- `cafe_menu.html` + `cafe_menu_styles.css` - A CSS styling project demonstrating layout, positioning, and responsive design
- `random.html` - Basic HTML structure practice with lists and paragraphs

## Architecture

This is a static HTML/CSS learning repository with no build system or framework dependencies. Each HTML file is self-contained and can be opened directly in a web browser for testing and viewing.

### Key Characteristics:
- **Static Files Only**: No server-side processing or JavaScript frameworks
- **Educational Purpose**: Focused on learning HTML and CSS fundamentals
- **Standalone Projects**: Each HTML file represents a separate learning exercise
- **External Resources**: Uses FreeCodeCamp CDN for images and styling assets

## Development Workflow

### Viewing Projects
```bash
# Open any HTML file directly in the default browser
open cafe_menu.html
open CatPhotoApp.html
open random.html

# Or use a simple HTTP server if needed
python3 -m http.server 8000
# Then visit http://localhost:8000/filename.html
```

### Live Development
For real-time editing and preview:
```bash
# Using Live Server (if installed globally)
live-server .

# Or with Python's built-in server
python3 -m http.server 8000
```

### File Validation
```bash
# Check HTML validation (requires html5validator)
html5validator --root . --also-check-css

# Basic syntax checking with built-in tools
find . -name "*.html" -exec echo "Checking {}" \; -exec head -1 {} \;
```

## Common Tasks

### Adding New Projects
1. Create new HTML file with proper DOCTYPE and structure
2. Link CSS file using relative path: `<link rel="stylesheet" href="filename.css">`
3. Follow the existing pattern of semantic HTML structure

### CSS Organization
- Keep CSS files separate from HTML
- Use class-based styling following the existing patterns
- Maintain consistent naming conventions (kebab-case for classes)

### Testing Changes
Simply refresh the browser after making changes to HTML or CSS files. No build process is required.

## Project-Specific Notes

### CatPhotoApp.html
- Comprehensive HTML learning project
- Covers forms, semantic HTML, images, links, and lists
- Uses external FreeCodeCamp images and resources

### Cafe Menu Project
- Demonstrates CSS layout techniques
- Uses background images from FreeCodeCamp CDN
- Shows inline-block positioning and text alignment

### Random.html
- Basic HTML structure practice
- Simple list and paragraph elements
- Minimal styling for fundamental learning
