<div align="center">
  <h1>README Motion</h1>
  <p><strong>Create an animated GitHub profile hero in under 60 seconds.</strong></p>
  <p>No design skills. No account. No build step.</p>
  <p>
    <a href="https://loccao102.github.io/readme-motion/"><strong>Open the studio →</strong></a>
    · <a href="#features">Features</a>
    · <a href="#local-development">Run locally</a>
  </p>
</div>

## Why

GitHub profiles are personal, but most README generators produce the same result. README Motion creates a lightweight animated SVG that can reflect your own voice, colors, and visual identity — and exports it with one line of Markdown.

## Features

- Live animated SVG preview.
- Five visual templates with distinct compositions.
- Custom copy, colors, motion speed, and corner icon.
- Optional avatar or mascot embedded directly into the SVG.
- Download SVG or copy the source.
- Copy-ready GitHub Markdown.
- Import/export configuration as JSON.
- Automatic local persistence.
- Accessible reduced-motion support.
- Fully client-side: your data and images never leave the browser.

## Use the exported hero

1. Download `hero.svg`.
2. Add it to `assets/hero.svg` in your profile repository.
3. Paste this into `README.md`:

```html
<img width="100%" src="./assets/hero.svg" alt="Animated profile hero" />
```

## Local development

There is no framework and no dependency installation. Serve the repository with any static server:

```bash
python -m http.server 4173
```

Open `http://localhost:4173`.

Run the tests with Node.js 20 or newer:

```bash
npm test
npm run check
```

## Project structure

```text
readme-motion/
├── index.html
├── styles.css
├── src/
│   ├── app.js
│   └── svg-generator.js
├── tests/
│   └── svg-generator.test.js
└── .github/workflows/pages.yml
```

## Roadmap

- Shareable configuration URLs.
- More compositions and typography controls.
- GitHub Action for automatic regeneration.
- CLI and reusable rendering package.
- Community template gallery.

Contributions and template ideas are welcome.

## License

[MIT](./LICENSE) © Cao Tien Loc
