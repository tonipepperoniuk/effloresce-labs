# Effloresce Labs Website

One-page static website for Effloresce Labs.

## Local preview
Open `index.html` in your browser.

## GitHub Pages & CI/CD

This website is automatically built and deployed to GitHub Pages using GitHub Actions (`.github/workflows/deploy.yml`).

### Workflow Details
- **Pull Requests**: Pull requests targeting `main` automatically run the `build-and-validate` job to verify static files, asset references, and build integrity without deploying to live.
- **Publishing (`main`)**: Merging or pushing to `main` executes validation and publishes the site directly to GitHub Pages (`efflorescelabs.com`).
- **Manual Trigger**: Can also be triggered manually via GitHub Actions **Run workflow** (`workflow_dispatch`).

### GitHub Repository Setup
In repository settings:
1. Go to **Settings** > **Pages**
2. Under **Build and deployment** > **Source**, select **GitHub Actions**
