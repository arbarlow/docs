# CLAUDE.md

## Project Overview

This is a Mintlify-based documentation site for Stride, a cycling and endurance training platform. The documentation uses MDX files (Markdown with JSX components) and is configured via `docs.json`.

## Essential Commands

```bash
# Run local development server
mintlify dev

# Troubleshooting - reinstall dependencies
mintlify install
```

## Architecture

### Framework
- **Mintlify**: Modern documentation framework that handles build, deployment, and hosting
- **MDX**: All content files use .mdx extension (Markdown + JSX components)
- **No build configuration**: Mintlify handles everything internally

### Key Files
- `docs.json`: Central configuration defining navigation, theme, and site metadata
- `index.mdx`: Homepage with hero sections and feature cards
- Content organized in topic-based folders (getting-started/, training/, etc.)

### Navigation Structure
The site has two main tabs defined in `docs.json`:
1. **Guides**: Step-by-step instructions and feature documentation
2. **Reference**: FAQs and glossary

### Reference
The main product is usually located at @../stride (backend), @../stride-web (frontend), and @../stride-mobile (mobile app). You can use these codebases to get insight into available features, limitations etc

### Deployment
- Automatic deployment via GitHub integration
- Push to main branch triggers deployment
- No manual build process required
