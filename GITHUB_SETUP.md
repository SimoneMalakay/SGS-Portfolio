# GitHub Repository Setup Guide

Your portfolio website is ready! Follow these steps to create the GitHub repository and connect it to Netlify.

## Step 1: Create GitHub Repository

1. Go to [GitHub](https://github.com) and sign in
2. Click the "+" icon in the top right corner
3. Select "New repository"
4. Repository name: `sgs-portfolio` (or your preferred name)
5. Description: "Portfolio website for Simone Greco Solutions"
6. Set visibility: Public or Private (your choice)
7. **DO NOT** initialize with README, .gitignore, or license (we already have these)
8. Click "Create repository"

## Step 2: Connect Local Repository to GitHub

After creating the repository on GitHub, run these commands in your terminal:

```bash
cd /Users/simonegreco/sgs-portfolio

# Add the remote repository (replace YOUR_USERNAME with your GitHub username)
git remote add origin https://github.com/YOUR_USERNAME/sgs-portfolio.git

# Push to GitHub
git branch -M main
git push -u origin main
```

## Step 3: Deploy to Netlify

1. Go to [Netlify](https://app.netlify.com) and sign in
2. Click "Add new site" → "Import an existing project"
3. Choose "GitHub" as your Git provider
4. Authorize Netlify to access your GitHub repositories
5. Select the `sgs-portfolio` repository
6. Netlify will auto-detect the settings:
   - Build command: (leave empty)
   - Publish directory: `.` (current directory)
7. Click "Deploy site"

## Step 4: Continuous Deployment

Once connected, every time you push changes to the `main` branch on GitHub, Netlify will automatically rebuild and deploy your site!

## Quick Commands Reference

```bash
# Make changes to your files, then:
git add .
git commit -m "Your commit message"
git push origin main
```

That's it! Your site will be live and automatically updated.

