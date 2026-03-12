# tom-and-jerry Website

Marketing and documentation site for the tom-and-jerry open protocol.

## About tom-and-jerry

tom-and-jerry is an open protocol for connecting AI agents across your machines. Tom orchestrates. Jerry computes. You just describe the task.

- **Tom**: Always-on orchestrator (cloud/Linux)
- **Jerry**: GPU compute node that wakes on demand (home PC/Windows)
- **CLI**: `tj`

## Tech Stack

- **Astro** - Static site generator
- **Tailwind CSS** - Styling
- **Vercel** - Deployment

## Development

```bash
# Install dependencies
npm install

# Start dev server
npm run dev

# Build for production
npm run build

# Preview production build
npm run preview
```

## Deploy

### Vercel (Recommended)

1. Connect this repo to Vercel
2. Vercel will auto-detect Astro
3. Deploy

Or use the Vercel CLI:

```bash
npm install -g vercel
vercel
```

### Other platforms

Build the static site:

```bash
npm run build
```

The output in `dist/` can be deployed to any static hosting provider (Netlify, Cloudflare Pages, GitHub Pages, etc.).

## Project Structure

```
├── src/
│   ├── layouts/
│   │   └── Layout.astro       # Shared layout with nav + footer
│   ├── pages/
│   │   ├── index.astro        # Homepage
│   │   ├── install.astro      # Install guide
│   │   ├── hardware.astro     # Hardware profiles
│   │   └── docs/
│   │       └── index.astro    # CLI docs
│   └── styles/
│       └── global.css         # Global styles + theme
├── public/                    # Static assets
└── vercel.json               # Vercel config
```

## Design

Dark terminal aesthetic inspired by Railway.app, Warp.dev, and Linear.

**Color palette:**
- Background: #0a0a0a
- Surface: #111111
- Border: #222222
- Primary: #ff6b35 (orange-red — Tom is a fire demon)
- Secondary: #4ade80 (green — terminal output)
- Text: #e5e5e5
- Muted: #666666

**Fonts:**
- Body: Inter / system-ui
- Code: JetBrains Mono / monospace

## License

MIT
