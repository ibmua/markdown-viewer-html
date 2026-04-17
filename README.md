# markdown-viewer-html

A single-file, zero-install markdown viewer. Open `index.html` in any browser,
drag `.md` files onto the page, and read them rendered — GitHub-style, with
dark mode, syntax highlighting, and tables.

No build step, no server, no upload: everything runs locally in the browser.

## Features

- **Drag & drop** one or many `.md` files anywhere on the page
- **File picker** (`Open files…`) for the clicky crowd
- **Paste markdown** from the clipboard with <kbd>⌘V</kbd> / <kbd>Ctrl</kbd>+<kbd>V</kbd>
- **Multi-file sidebar** — stack files, switch between them, close individually
- GitHub-flavored markdown: tables, task lists, fenced code blocks, footnotes
- Syntax highlighting (highlight.js)
- Light / dark theme follows your OS
- HTML sanitized with DOMPurify before rendering

## Use

1. Download / clone this repo
2. Double-click `index.html`

Or just open the hosted copy on GitHub Pages (enable Pages → root / main).

## Keyboard shortcuts

| Shortcut | Action |
|---|---|
| <kbd>⌘</kbd>+<kbd>O</kbd> / <kbd>Ctrl</kbd>+<kbd>O</kbd> | Open files |
| <kbd>⌘</kbd>+<kbd>W</kbd> / <kbd>Ctrl</kbd>+<kbd>W</kbd> | Close active file |
| <kbd>⌘</kbd>+<kbd>V</kbd> / <kbd>Ctrl</kbd>+<kbd>V</kbd> | Paste markdown as a new file |

## Dependencies

Loaded at runtime from jsDelivr CDN:

- [marked](https://github.com/markedjs/marked) — markdown → HTML
- [DOMPurify](https://github.com/cure53/DOMPurify) — XSS sanitization
- [highlight.js](https://github.com/highlightjs/highlight.js) — code blocks

Nothing is bundled; your browser pulls them on first open and caches them.
If you need fully offline use, vendor the three scripts into the repo and
update the `<script>` / `<link>` tags accordingly.

## License

MIT — see [LICENSE](LICENSE).
