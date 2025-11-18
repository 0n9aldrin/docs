# PhotoMem Documentation

Complete documentation for PhotoMem - a production-grade memory layer for AI agents.

## 📁 Structure

```
docs/
├── docs.json                 # Configuration
├── styles.css                # Custom styling
├── index.mdx                 # Homepage
├── introduction.mdx          # Overview
├── quickstart.mdx            # Quick start guide
├── installation.mdx          # Installation
├── core-concepts.mdx         # Core concepts
├── development.mdx           # Development guide
├── api-reference/            # API documentation
│   ├── introduction.mdx      # API overview
│   ├── memory.mdx            # Memory class methods
│   ├── types.mdx             # Type definitions
│   ├── errors.mdx            # Error handling guide
│   ├── rest-api.mdx          # REST API endpoints
│   └── openapi.json          # OpenAPI spec
├── examples/                 # Code examples
│   ├── python.mdx            # Python examples
│   └── README.md
├── ai-tools/                 # AI assistant configs
│   ├── cursor.mdx
│   ├── windsurf.mdx
│   └── claude-code.mdx
├── images/                   # Images
├── logo/                     # Logo files
└── snippets/                 # Reusable snippets
```

## 🎯 Content Overview

### Getting Started
- **index.mdx** - Homepage with hero section
- **introduction.mdx** - Project overview and features
- **quickstart.mdx** - 5-minute tutorial
- **installation.mdx** - Setup for Python/TypeScript

### Core Documentation
- **core-concepts.mdx** - Memory types, semantic search, deduplication, etc.
- **development.mdx** - Local development setup

### API Reference
- **memory.mdx** - Complete Memory class documentation with all methods
- **types.mdx** - All type definitions for Python and TypeScript
- **errors.mdx** - Error handling guide with examples
- **rest-api.mdx** - HTTP API endpoints and authentication

### Examples
- **python.mdx** - Real-world Python examples
- **typescript_example.ts** - TypeScript code samples

### AI Tools
- **cursor.mdx** - Cursor AI configuration
- **windsurf.mdx** - Windsurf Cascade setup
- **claude-code.mdx** - Claude Code usage

## 🎨 Custom Styling

The docs use a custom dark theme defined in `styles.css`:

### Colors
- **Background**: Navy (`#0A0F1E`)
- **Primary**: Cyan (`#00D9FF`)
- **Secondary**: Purple
- **Accent**: Pink

### Features
- Glass morphism effects
- Custom scrollbars
- Gradient backgrounds
- Smooth animations

## 📝 Writing Guidelines

### MDX Format

All pages use MDX (Markdown + JSX):

```mdx
---
title: 'Page Title'
description: 'Page description'
icon: 'icon-name'
---

## Section

Content here...

<Card title="Feature" icon="star">
  Card content
</Card>
```

### Components

Available components:

```mdx
# Cards
<Card title="Title" icon="rocket" href="/link">
  Content
</Card>

<CardGroup cols={2}>
  <Card>...</Card>
  <Card>...</Card>
</CardGroup>

# Code Blocks
<CodeGroup>
```python
# Python
```

```typescript
// TypeScript
```
</CodeGroup>

# Tabs
<Tabs>
  <Tab title="Python">
    Python content
  </Tab>
  <Tab title="TypeScript">
    TypeScript content
  </Tab>
</Tabs>

# Callouts
<Note>Note message</Note>
<Info>Info message</Info>
<Warning>Warning message</Warning>
<Tip>Tip message</Tip>

# Expandable
<Accordion title="Click to expand">
  Hidden content
</Accordion>
```

## 📋 Configuration

### docs.json

Main configuration file:

```json
{
  "name": "PhotoMem",
  "logo": {
    "dark": "/logo/dark.png",
    "light": "/logo/light.png"
  },
  "favicon": "/favicon.svg",
  "colors": {
    "primary": "#00D9FF",
    "light": "#00D9FF",
    "dark": "#0A0F1E"
  },
  "navigation": [...]
}
```

## 🚀 Content Best Practices

### 1. Code Examples

Always provide both Python and TypeScript:

```mdx
<Tabs>
  <Tab title="Python">
    ```python
    from photomem import Memory
    ```
  </Tab>
  <Tab title="TypeScript">
    ```typescript
    import { Memory } from 'photomem';
    ```
  </Tab>
</Tabs>
```

### 2. API Documentation

Include:
- Method signature
- Parameters with types
- Return values
- Error cases
- Examples

### 3. User IDs

Always use the format `phone:15103651277` in examples.

### 4. Visual Hierarchy

- Use headers (`##`, `###`) for structure
- Use callouts for important info
- Use cards for feature highlights
- Use tables for comparisons

## 📦 Navigation Updates

To add a new page to `docs.json`:

```json
{
  "group": "API Reference",
  "pages": [
    "api-reference/introduction",
    "api-reference/memory",
    "api-reference/types",
    "api-reference/errors",
    "api-reference/rest-api",
    "api-reference/new-page"  // Add here
  ]
}
```

## 🔍 Search

Search is automatic and indexes:
- Page titles
- Headers
- Content text
- Code blocks

## 📱 Responsive Design

Documentation is fully responsive:
- Mobile-friendly navigation
- Collapsible sidebar
- Touch-friendly buttons
- Readable code blocks

## 🎯 Content Strategy

### Primary Audience
- Backend developers
- AI/ML engineers
- Full-stack developers

### Key Messages
1. Production-ready
2. Type-safe
3. High-performance
4. Easy to use

### Content Types
- **Tutorials** - Step-by-step guides
- **Reference** - API documentation
- **Explanations** - Concepts and architecture
- **Examples** - Real-world use cases

## ✅ Quality Checklist

Before publishing new content:

- [ ] All code examples tested
- [ ] Both Python and TypeScript examples
- [ ] Clear, descriptive headings
- [ ] Callouts for important info
- [ ] Links work correctly
- [ ] Images have alt text
- [ ] Proper formatting
- [ ] No spelling errors

## 🔗 Internal Linking

Use relative paths:

```mdx
See [Core Concepts](/core-concepts) for details.
Link to [Memory API](/api-reference/memory)
```

## 📊 Analytics

Track:
- Page views
- Search queries
- Popular pages
- User flows

## 🎓 Learning Path

Recommended order:
1. Introduction
2. Quick Start
3. Installation
4. Core Concepts
5. API Reference
6. Examples

## 🤝 Contributing

To contribute:
1. Edit `.mdx` files
2. Test locally
3. Submit PR
4. Auto-deploys on merge

## 📞 Support

For documentation issues:
- Open GitHub issue
- Contact team
- Check existing docs

---

**Happy documenting!** 📚
