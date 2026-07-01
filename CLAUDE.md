# CLAUDE.md

## Project Overview

This repository contains interactive HTML widgets created by AI for teaching technology courses — primarily Machine Learning, Artificial Intelligence, and related areas. Each widget is a self-contained, standalone HTML file with embedded CSS and JavaScript (no build step needed).

## Deployment

- **GitHub Pages**: `https://mtgca.github.io/widgets_pubic/`
- **Entry point**: `README.md` (rendered as the GitHub Pages index via the default Jekyll theme)
- Pushing to `main` automatically deploys to GitHub Pages.

## Repository Structure

```
widgets_pubic/
├── README.md                          # Entry point / index page
├── CLAUDE.md                          # This file
├── llmpretraining.html                # LLM next-word prediction
├── external_metrics_interactive.html  # Clustering evaluation metrics (ARI & NMI)
├── gmm_covariance_interactive.html    # GMM covariance types
├── gmm_em_interactive.html            # EM algorithm for GMMs
└── linkage_methods_interactive.html   # Hierarchical clustering linkage methods
```

## Widget Conventions

- Each widget is a **single, self-contained `.html` file** — no external dependencies, no build tools.
- Widgets embed all CSS and JS inline so they work when served directly from GitHub Pages.
- Widget filenames should be descriptive and end in `_interactive.html` for interactive demos, or be clearly named for the concept they teach.
- When adding a new widget, **both** `README.md` and `index.html` must be updated (see below).
- Every widget carries a **verification badge** (`data-verified`) indicating whether a human expert has reviewed it; new widgets start `"false"` (see "Human-Expert Verification").

## Courses Covered

- **Machine Learning**: clustering algorithms, model evaluation metrics, probabilistic models
- **Artificial Intelligence / Deep Learning**: LLM pretraining, neural networks
- Other technology areas as needed

## Adding a New Widget

1. Create a self-contained `.html` file in the repo root.
2. Keep all CSS and JS inline (no CDN dependencies when avoidable).
3. Add the **verification badge** snippet immediately after `<body>`, with `data-verified="false"` (see below). Every new widget starts unverified.
4. Add a row to the table of contents in `README.md` with the GitHub Pages URL, a one-line description, and a `⚠️ AI-only` Status cell.
5. Add a card to `index.html` inside the `#grid` div, following the existing card pattern (`data-verified="false"` on the `<a class="card">`, tags, title, desc, `<span class="verify-badge"></span>`, arrow link).
6. Commit and push — GitHub Pages deploys automatically.

> **Important**: Steps 4 and 5 are both required every time a widget is added. Never update one without the other.

## Human-Expert Verification

Widgets are AI-generated. A widget is only marked **verified** once a human expert in the field has reviewed it for correctness. Until then it shows an explicit caution label so users take it with a grain of salt.

Status is tracked by a single `data-verified` attribute (`"true"` / `"false"`) in three places per widget:

- **Inside the widget** — the `.verify-badge` snippet after `<body>` renders a fixed corner pill: green `✓ Expert-verified` or amber `⚠ AI-generated · not expert-verified`. The badge uses `pointer-events:none`; if it overlaps a widget's own top-right controls, move it to `top:10px;left:10px` in that file only.
- **`index.html`** — `data-verified` on the card's `<a>` drives the card badge via CSS, and powers the **✓ Verified** filter.
- **`README.md`** — the Status column cell: `✅ Verified` or `⚠️ AI-only`.

**To mark a widget verified**, flip all three: `data-verified="true"` in the widget file, `data-verified="true"` on its `index.html` card, and the README Status cell to `✅ Verified`.
