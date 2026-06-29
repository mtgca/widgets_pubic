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

## Courses Covered

- **Machine Learning**: clustering algorithms, model evaluation metrics, probabilistic models
- **Artificial Intelligence / Deep Learning**: LLM pretraining, neural networks
- Other technology areas as needed

## Adding a New Widget

1. Create a self-contained `.html` file in the repo root.
2. Keep all CSS and JS inline (no CDN dependencies when avoidable).
3. Add a row to the table of contents in `README.md` with the GitHub Pages URL and a one-line description.
4. Add a card to `index.html` inside the `#grid` div, following the existing card pattern (tags, title, desc, arrow link).
5. Commit and push — GitHub Pages deploys automatically.

> **Important**: Steps 3 and 4 are both required every time a widget is added. Never update one without the other.
