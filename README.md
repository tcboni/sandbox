# Sandbox

A lightweight in-browser sandbox for editing HTML, CSS, and JavaScript with live preview, syntax highlighting, shareable URLs, and an integrated console.

**[→ Open Sandbox](https://tcboni.github.io/sandbox/)**

## Features

- Three resizable editors for HTML, CSS, and JavaScript
- Live preview with throttled updates while typing
- Syntax highlighting powered by Highlight.js
- Built-in console panel for `log`, `warn`, `error`, and `info`
- Share button that encodes editor state into the URL hash
- Persistent local state (code, panel sizes, console visibility)
- GitHub repo shortcut in the header

## How It Works

- Editor code is stored in browser localStorage.
- Preview is rendered into an iframe using `srcdoc`.
- Console messages are forwarded from the iframe to the parent window with `postMessage`.
- Syntax highlighting uses CDN-hosted Highlight.js assets.

## Project Structure

- `index.html` - Entire app (layout, styles, and JavaScript logic)
