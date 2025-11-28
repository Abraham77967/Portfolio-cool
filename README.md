<div align="center">
<img width="1200" height="475" alt="GHBanner" src="https://github.com/user-attachments/assets/0aa67016-6eaf-458a-adb2-6e31a0763ed6" />
</div>

# Portfolio Website

A React + TypeScript portfolio website built with Vite.

## Run Locally

**Prerequisites:** Node.js

1. Install dependencies:
   ```bash
   npm install
   ```
2. Set the `GEMINI_API_KEY` in `.env.local` to your Gemini API key (if needed)
3. Run the app:
   ```bash
   npm run dev
   ```

## Deploy to GitHub Pages

This project is configured to automatically deploy to GitHub Pages using GitHub Actions.

### Setup Instructions:

1. **Push your code to GitHub:**
   ```bash
   git init
   git add .
   git commit -m "Initial commit"
   git branch -M main
   git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git
   git push -u origin main
   ```

2. **Enable GitHub Pages:**
   - Go to your repository on GitHub
   - Click on **Settings** → **Pages**
   - Under **Source**, select **GitHub Actions** (not "Deploy from a branch")
   - The workflow will automatically deploy on every push to `main` or `master` branch

3. **Access your site:**
   - Your site will be available at: `https://YOUR_USERNAME.github.io/YOUR_REPO_NAME/`
   - If you're using a custom domain or deploying to the root of your GitHub Pages site, update the `base` in `vite.config.ts` accordingly

### Manual Deployment:

If you prefer to deploy manually:
```bash
npm run build
# Then push the dist folder to the gh-pages branch
```

The GitHub Actions workflow will handle automatic deployments on every push to the main branch.
