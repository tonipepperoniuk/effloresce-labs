# Effloresce Labs Website

One-page static website for Effloresce Labs.

## Local Preview

You can preview the site locally using any of the following options:

### 1. Python Built-in Server (Recommended)
```bash
python3 -m http.server 8000
```
Open **[http://localhost:8000](http://localhost:8000)** in your browser.

### 2. Node / npx
```bash
npx serve .
```

### 3. Direct File
Open `index.html` directly in any web browser.

## GitHub Pages & CI/CD

This website is automatically built and deployed to GitHub Pages using GitHub Actions (`.github/workflows/deploy.yml`).

### Workflow Details
- **Branch Pushes & Pull Requests**: Pushing to any branch or opening a pull request targeting `main` automatically runs the `build-and-validate` job to verify static files, asset references, and build integrity without deploying to live.
- **Publishing (`main`)**: Pushing or merging directly to `main` executes validation and publishes the site directly to GitHub Pages (`efflorescelabs.com`).
- **Manual Trigger**: Can also be triggered manually via GitHub Actions **Run workflow** (`workflow_dispatch`).

### GitHub Repository Setup
In repository settings:
1. Go to **Settings** > **Pages**
2. Under **Build and deployment** > **Source**, select **GitHub Actions**
