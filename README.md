# vgoehler.github.io

My personal website built with [Quarto](https://quarto.org/).

## Setup

This repository is configured to automatically build and deploy a Quarto website using GitHub Actions.

### How It Works

1. Edit the `.qmd` files (Quarto Markdown) to update content
2. Push changes to the repository
3. GitHub Actions automatically builds the site using Quarto
4. The built website is committed to the `docs/` directory
5. GitHub Pages serves the site from the `docs/` directory

### Configuration

- `_quarto.yml` - Main Quarto configuration file
- `index.qmd` - Home page content
- `about.qmd` - About page content
- `.github/workflows/quarto-publish.yml` - GitHub Actions workflow

### GitHub Pages Setup

To enable GitHub Pages:

1. Go to repository Settings → Pages
2. Under "Source", select "Deploy from a branch"
3. Select the branch (main or your working branch) and `/docs` folder
4. Click Save

The site will be available at: https://vgoehler.github.io/

### Local Development

To build the site locally:

```bash
quarto render
```

This will generate the site in the `docs/` directory.
