# Monkey King Obsidian Theme

A custom Obsidian theme built with Sass.

## Development

### Prerequisites
- Node.js
- npm

### Setup
```bash
npm install
```

### Build
```bash
# Build once
npm run build

# Watch for changes
npm run watch
# or
npm run dev
```

### Installation
1. Copy the `theme.css` and `manifest.json` files to your Obsidian themes folder
2. Enable the theme in Obsidian settings

## File Structure
```
├── src/                 # Sass source files
│   └── main.scss       # Main Sass entry point
├── theme.css           # Compiled CSS (generated)
├── manifest.json       # Obsidian theme manifest
└── package.json        # Node.js dependencies
```