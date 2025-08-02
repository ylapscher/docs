# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is the Harbor Parking API documentation site built with Mintlify. It contains comprehensive REST API documentation for the Harbor Parking application, which enables parking spot sharing within residential communities.

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
- **Content**: MDX files with YAML frontmatter for API endpoint documentation
- **Structure**:
  - `/api-reference/` - All API documentation and endpoint examples
    - `/profile/` - User profile management endpoints
    - `/dashboard/` - Dashboard data endpoints
    - `/parking-spots/` - Parking spot CRUD operations
    - `/availabilities/` - Availability window management
    - `/claims/` - Parking spot reservation system
  - `/snippets/` - Reusable content snippets (auth warnings, etc.)
  - `/logo/` - Harbor Parking branding assets

## Content Standards

### MDX File Requirements
- YAML frontmatter with `title`, `description`, and `api` fields for endpoints
- Use Mintlify components (Card, CardGroup, Steps, ResponseField, etc.)
- Language tags on all code blocks
- Relative paths for internal links
- Consistent authentication snippets using `<Snippet file="auth-required.mdx" />`

### API Documentation Structure
- **Introduction** - API overview and getting started
- **Authentication** - JWT authentication guide
- **Quickstart** - Quick examples for common workflows
- **Endpoint Groups** - Organized by resource type (Profile, Parking Spots, etc.)
- Each endpoint includes: overview, auth requirements, parameters, response format, examples

### Navigation Structure
- Single-level navigation organized by functional groups
- No tabs - simplified structure focusing only on API reference
- Groups: Getting Started, Profile & Authentication, Dashboard, Parking Spots, Availabilities, Claims

## Branding
- **Name**: Harbor Parking API
- **Colors**: Blue theme (#3B82F6 primary, #60A5FA light, #1E40AF dark)
- **Theme**: "quill" for clean, professional appearance
- **Links**: Harbor Parking app and GitHub repository

## Prerequisites
- Node.js version 19 or higher
- Mintlify CLI (`npm i -g mint`)

## Deployment
- Local preview available at `http://localhost:3000`
- Deployed documentation should be hosted at a docs subdomain