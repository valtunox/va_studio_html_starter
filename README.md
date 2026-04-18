<p align="center">
  <img src="https://img.shields.io/badge/HTML-5-E34F26?style=for-the-badge&logo=html5&logoColor=white" alt="HTML5" />
  <img src="https://img.shields.io/badge/CSS-3-1572B6?style=for-the-badge&logo=css3&logoColor=white" alt="CSS3" />
  <img src="https://img.shields.io/badge/Zero_Build-Zero_Deps-22C55E?style=for-the-badge" alt="Zero build" />
  <img src="https://img.shields.io/badge/Studio_Builder-Ready-8B5CF6?style=for-the-badge" alt="Studio Builder Ready" />
  <img src="https://img.shields.io/badge/AI-Ready-F59E0B?style=for-the-badge" alt="AI Ready" />
</p>

<h1 align="center">VA Studio HTML Starter — Invoice</h1>

<p align="center">
  <strong>A print-ready, corporate-grade invoice template built with zero dependencies.</strong>
</p>

<p align="center">
  Drop-in HTML + CSS for generating professional invoices. Clean typography, sticky action bar, <br/>
  print stylesheet, and a layout that works equally well on screen and on paper.
</p>

<p align="center">
  <a href="#quick-start">Quick Start</a> &bull;
  <a href="#features">Features</a> &bull;
  <a href="#studio-builder-integration">Studio Integration</a> &bull;
  <a href="#customizing">Customizing</a>
</p>

---

## Quick Start

No build tools, no npm, no setup. Just open the file:

```bash
# Option 1 — double-click index.html
# Option 2 — serve with Python
python -m http.server 8000
# Option 3 — serve with Node
npx serve .
```

Then visit [http://localhost:8000](http://localhost:8000).

## Features

- **Print-Ready** — dedicated `@media print` stylesheet strips chrome for clean PDF output
- **Sticky Action Bar** — Email, Print, and Download-PDF actions always in reach
- **Payment Instructions** — bank routing, account, and reference number block
- **Line-Item Ledger** — description, quantity, unit rate, and amount per row
- **Auto-Calc Totals** — subtotal, discount, tax, and amount due — semantically structured
- **Digital Signature Line** — ready for e-signature overlays or Studio macros
- **Responsive** — collapses gracefully on mobile without losing print fidelity
- **Zero Dependencies** — no jQuery, no Bootstrap, no framework — just HTML + CSS

## Studio Builder Integration

Part of the **VA Studio** family and designed to be manipulated by the Studio Builder's AI layer:

- Every section has semantic class names — Studio AI can target `party`, `lines`, `totals`, `payment` safely
- Inline style usage is minimal so Studio's theme engine can re-skin without fighting overrides
- Works with `studio.go`'s static preview server — saves trigger an instant reload
- Metadata structure matches the Studio billing schema — fields map 1:1 to invoice objects

## Tech Stack

| Layer | Technology |
|-------|-----------|
| **Markup** | HTML5, semantic landmarks |
| **Styling** | CSS3 custom properties, print media queries |
| **Fonts** | Inter + Playfair Display (Google Fonts) |
| **Icons** | Inline SVG — no icon library needed |

## Project Structure

```
va_studio_html_starter/
├── index.html      # Invoice markup
├── styles.css      # Design tokens + print stylesheet
└── README.md
```

## Customizing

- **Brand:** edit the `.brand-block` in `index.html` — logo is an inline SVG
- **Colors:** update CSS custom properties at the top of `styles.css` (`--ink-900`, `--accent`, `--success`)
- **Currency & Locale:** numbers are plain text — swap in your locale formatting or Studio bindings
- **Line items:** `<tbody>` rows in the `.lines` table — AI-generated items slot in cleanly

## License

MIT

---

<p align="center">
  Part of the <strong>VA Studio</strong> starter family · Built for rapid prototyping with an AI copilot.
</p>
