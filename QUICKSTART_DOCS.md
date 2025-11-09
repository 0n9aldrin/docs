# Quick Start - PhotoMem Documentation

## 🚀 Get Started in 3 Commands

```bash
# 1. Install Mintlify CLI
npm install -g mintlify

# 2. Navigate to docs
cd /Users/aldrin0n9/Developer/daymi/photomem/docs

# 3. Start dev server
mintlify dev
```

Then open: **http://localhost:3000**

---

## 📚 What You'll See

Your documentation includes:

✅ **Landing Page** - Hero with benchmarks  
✅ **Quick Start** - 5-minute tutorial  
✅ **Installation** - Complete setup guide  
✅ **Core Concepts** - Memory types, IDs, search  
✅ **API Reference** - Methods and types  
✅ **Python Examples** - 10+ real-world examples  

All with your **custom dark theme** (navy + cyan + glass effects)!

---

## 🎨 Your Theme

Colors applied:
- Background: Navy (`#0A0F1E`)
- Primary: Cyan (`#00D9FF`)
- Glass surfaces with backdrop blur
- Custom scrollbars

---

## 📖 Documentation Structure

```
docs/
├── introduction.mdx     # Landing page
├── quickstart.mdx       # Quick start
├── installation.mdx     # Install guide
├── core-concepts.mdx    # Concepts
├── api-reference/
│   └── introduction.mdx # API overview
└── examples/
    └── python.mdx       # Python examples
```

---

## 🔧 Common Tasks

### Preview Changes
```bash
mintlify dev
```

### Add New Page
1. Create `my-page.mdx` in docs/
2. Add to `mint.json` navigation:
```json
{
  "group": "Group Name",
  "pages": ["my-page"]
}
```

### Deploy
1. Sign up at mintlify.com
2. Connect GitHub repo
3. Auto-deploys on push to main

---

## 📋 Quick Reference

### Components

```mdx
<Card title="Title" icon="rocket" href="/link">
  Content
</Card>

<CodeGroup>
```python
# Python code
```

```typescript
// TypeScript code
```
</CodeGroup>

<Note>Note message</Note>
<Warning>Warning message</Warning>
<Info>Info message</Info>
```

---

## ✅ You're All Set!

Run `mintlify dev` and your beautiful documentation will be live at http://localhost:3000

Need help? Check:
- `DOCS_README.md` - Full documentation guide
- `DOCUMENTATION_SUMMARY.md` - Complete summary
- [Mintlify Docs](https://mintlify.com/docs)

