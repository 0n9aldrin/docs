# PhotoMem Documentation

This directory contains the **Mintlify documentation** for PhotoMem.

## 📚 Documentation Structure

```
docs/
├── mint.json                 # Mintlify configuration
├── styles.css               # Custom dark theme styles
├── introduction.mdx         # Landing page
├── quickstart.mdx           # Quick start guide
├── installation.mdx         # Installation instructions
├── core-concepts.mdx        # Core concepts explained
├── api-reference/           # API documentation
│   └── introduction.mdx     # API overview
└── examples/                # Practical examples
    └── python.mdx          # Python examples
```

## 🎨 Theme

The documentation uses your custom dark theme with:
- **Background**: Navy (`hsl(210 50% 5%)`)
- **Primary/Accent**: Cyan (`hsl(184 100% 50%)`)
- **Glass surface effects** with backdrop blur
- **Custom scrollbars**
- **Smooth animations** (respecting prefers-reduced-motion)

## 🚀 Running Locally

### Prerequisites

```bash
npm install -g mintlify
```

### Start Development Server

```bash
cd /Users/aldrin0n9/Developer/daymi/photomem/docs
mintlify dev
```

Then open http://localhost:3000

## 📝 What's Included

### ✅ Complete Pages

1. **introduction.mdx** - Landing page with:
   - Hero section
   - Feature cards
   - Performance benchmarks
   - Quick example
   - Use cases

2. **quickstart.mdx** - Quick start guide with:
   - Prerequisites
   - Installation steps
   - First memory example (Python & TypeScript)
   - Understanding output
   - Next steps

3. **installation.mdx** - Installation guide with:
   - System requirements
   - Python & TypeScript installation
   - Database setup (Docker, manual, cloud)
   - Environment configuration
   - Verification steps
   - Troubleshooting

4. **core-concepts.mdx** - Core concepts with:
   - Memory types (Semantic, Episodic, Procedural)
   - User identifiers
   - Message formats
   - Metadata
   - Semantic search
   - Memory lifecycle
   - History tracking
   - Performance concepts
   - Best practices

5. **api-reference/introduction.mdx** - API overview with:
   - Quick reference table
   - Response formats
   - Error handling
   - Type safety
   - Authentication
   - Rate limits

6. **examples/python.mdx** - Python examples with:
   - Basic usage
   - Conversation memory
   - Custom configuration
   - Metadata and tagging
   - Batch operations
   - CRUD operations
   - Real-world examples (Personal assistant, Customer support, Multi-agent)
   - Performance monitoring
   - Error handling

### 🚧 To Be Created

Additional pages to complete the documentation:

```
guides/
├── configuration.mdx        # Configuration guide
├── memory-types.mdx        # Memory types deep dive
├── searching.mdx           # Search techniques
├── metadata.mdx            # Metadata usage
├── performance.mdx         # Performance optimization
└── error-handling.mdx      # Error handling guide

deployment/
├── docker.mdx              # Docker deployment
├── production.mdx          # Production setup
└── scaling.mdx             # Scaling strategies

api-reference/
├── memory.mdx              # Memory class methods
├── types.mdx               # Type definitions
├── errors.mdx              # Error reference
└── rest-api.mdx           # REST API endpoints

examples/
├── typescript.mdx          # TypeScript examples
├── personal-assistant.mdx  # Personal AI assistant
├── customer-support.mdx    # Customer support system
├── multi-agent.mdx         # Multi-agent systems
└── healthcare.mdx          # Healthcare application

advanced/
├── architecture.mdx        # Architecture deep dive
├── benchmarks.mdx          # Performance benchmarks
├── contributing.mdx        # Contributing guide
└── migration-from-mem0.mdx # Migration guide
```

## 🎨 Styling

The documentation uses your custom theme defined in `styles.css`:

### Color Palette

```css
--background: 210 50% 5%;      /* Navy background */
--foreground: 210 40% 98%;     /* Light text */
--primary: 184 100% 50%;       /* Cyan accent */
--secondary: 210 30% 15%;      /* Dark navy */
--border: 210 30% 20%;         /* Subtle borders */
```

### Utilities

```css
.glass-surface {
  @apply bg-white/6 backdrop-blur-xl border border-white/15;
}

.glass-surface-light {
  @apply bg-slate-900/10 backdrop-blur-xl border border-slate-900/15;
}
```

## 📦 Mintlify Configuration

Key configuration in `mint.json`:

```json
{
  "colors": {
    "primary": "#00D9FF",
    "light": "#00D9FF",
    "dark": "#00D9FF",
    "background": {
      "dark": "#0A0F1E"
    }
  },
  "tabs": [
    { "name": "API Reference", "url": "api-reference" },
    { "name": "Examples", "url": "examples" }
  ]
}
```

## 🔧 Customization

### Add New Page

1. Create MDX file (e.g., `guides/my-guide.mdx`)
2. Add frontmatter:
```mdx
---
title: My Guide
description: 'Guide description'
---
```
3. Add to navigation in `mint.json`:
```json
{
  "group": "Guides",
  "pages": ["guides/my-guide"]
}
```

### Add Code Examples

Use CodeGroup for multi-language:

```mdx
<CodeGroup>
```python Python
# Python code
```

```typescript TypeScript
// TypeScript code
```
</CodeGroup>
```

### Add Components

Mintlify provides built-in components:

```mdx
<Card title="Title" icon="rocket" href="/link">
  Description
</Card>

<Accordion title="Title" icon="info">
  Content
</Accordion>

<Note>Important note</Note>
<Warning>Warning message</Warning>
<Info>Information</Info>
<Check>Success message</Check>
```

## 📊 Analytics

To add analytics, update `mint.json`:

```json
{
  "analytics": {
    "ga4": {
      "measurementId": "G-XXXXXXXXXX"
    }
  }
}
```

## 🚀 Deployment

### Deploy to Mintlify

1. Sign up at [mintlify.com](https://mintlify.com)
2. Connect your GitHub repository
3. Mintlify auto-deploys on push to main

### Custom Domain

In Mintlify dashboard:
1. Settings → Custom Domain
2. Add your domain
3. Update DNS records

## 🎯 Next Steps

To complete the documentation:

1. Create remaining pages (see "To Be Created" section above)
2. Add more real-world examples
3. Create video tutorials
4. Add interactive demos
5. Build API playground
6. Add changelog page
7. Create migration guides

## 📞 Support

For Mintlify-specific questions:
- [Mintlify Documentation](https://mintlify.com/docs)
- [Mintlify Discord](https://discord.gg/mintlify)

For PhotoMem documentation questions:
- Open an issue on GitHub
- Join our Discord (coming soon)

