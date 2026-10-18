# Mini Split Flap

A realistic interactive split-flap display simulator that runs entirely in your browser. Inspired by the mechanical departure boards found in train stations and airports worldwide.

**[minisplitflap.com](https://minisplitflap.com)**

## Features

- **Realistic animation** — instanced WebGL renderer (DOM/CSS fallback) with gravity-based flap physics: drum release, free-fall, impact bounce, dynamic lighting and cast shadows
- **Fast** — one draw call renders 1000+ tiles at full frame rate; sounds play at the moment of card impact
- **Mechanical sound** — Web Audio API synthesis with configurable tone, snap, and body, glued by a master compressor
- **Sound presets** — Waterfall, Mechanical, Soft, Crisp, Heavy
- **Customizable scenes** — Write your own messages with text and shape syntax (`{heart}`, `{star}`, `{arrow}`, etc.)
- **Live data scenes** — Real-time clock, local weather (Open-Meteo), and stock market indices
- **Animation directions** — Left-to-right, diagonal, center-out, random, and more
- **Themes** — Charcoal, Midnight, Warm, Terminal
- **Auto-rotate** — Cycle through scenes like a slideshow
- **Fully responsive** — Scales to fit any screen size
- **Zero dependencies** — Single HTML file, no build step, no server required
- **Persistent settings** — Everything saves to localStorage

## Quick Start

Open `index.html` in any modern browser. That's it.

## Usage

- Click the **gear icon** (top-right) to open settings
- Select a scene from the list, or click **+ Add Scene** to create your own
- Use `{shapeName}` syntax for inline shapes: `{triangle}`, `{heart}`, `{star}`, `{diamond}`, `{arrow}`, `{circle}`, `{square}`, `{check}`, `{x}`
- Use **left/right arrow keys** to cycle through scenes
- Adjust flip speed, stagger, jitter, direction, and sound to taste

## Hosting

Single file — deploy anywhere that serves static files:

```bash
# GitHub Pages
gh repo create mini-split-flap --public --source=. --push
# Then enable Pages in repo Settings

# Or just a local server
python3 -m http.server 8080
```

## License

MIT
