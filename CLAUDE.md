# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a Mintlify documentation site using MDX files with YAML frontmatter. The site follows the Mintlify Starter Kit structure and includes documentation on AI tools like Claude Code, Cursor, and Windsurf.

## Commands

### Development
```bash
# Install Mintlify CLI globally
npm i -g mint

# Start local development server
mint dev

# Use custom port
mint dev --port 3333

# Update CLI to latest version
mint update
```

### Validation and Links
```bash
# Check for broken links
mint broken-links
```

## Architecture

- **Configuration**: `docs.json` - Controls navigation, theme, colors, and site settings
- **Content**: MDX files with YAML frontmatter in organized directories
- **Structure**:
  - `/ai-tools/` - Documentation for AI development tools
  - `/api-reference/` - API documentation and endpoint examples  
  - `/essentials/` - Core documentation features (markdown, code, images, etc.)
  - `/snippets/` - Reusable content snippets
  - `/images/` and `/logo/` - Static assets

## Content Standards

### MDX File Requirements
- YAML frontmatter with `title` and `description` fields
- Use Mintlify components (Card, CardGroup, Steps, etc.)
- Language tags on all code blocks
- Relative paths for internal links

### Navigation Structure
- Configured in `docs.json` under `navigation.tabs`
- Two main tabs: "Guides" and "API reference"
- Groups organize related pages within tabs

## Prerequisites
- Node.js version 19 or higher
- Mintlify CLI (`npm i -g mint`)

## Deployment
- Automatic deployment via Mintlify GitHub app
- Push to main branch triggers production deployment
- Local preview available at `http://localhost:3000`