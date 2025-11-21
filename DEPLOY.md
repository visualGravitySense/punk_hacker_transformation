# 🚀 Deployment Guide - GitHub Pages

This guide will help you deploy the Punk Hacker Transformation app to GitHub Pages.

## 📋 Prerequisites

- A GitHub account
- Repository: `visualGravitySense/punk_hacker_transformation`
- Push access to the repository

## 🔧 Setup Steps

### Step 1: Enable GitHub Pages

1. Go to your repository: https://github.com/visualGravitySense/punk_hacker_transformation
2. Click on **Settings** (in the repository navigation bar)
3. Scroll down to **Pages** in the left sidebar
4. Under **Source**, select:
   - **Source**: `Deploy from a branch`
   - **Branch**: `main`
   - **Folder**: `/ (root)`
5. Click **Save**

### Step 2: Verify GitHub Actions Workflow

The repository already includes a GitHub Actions workflow (`.github/workflows/deploy.yml`) that will automatically deploy your site when you push to the `main` branch.

### Step 3: Push Your Code

If you haven't already, commit and push all files:

```bash
git add .
git commit -m "Add GitHub Pages deployment"
git push origin main
```

### Step 4: Wait for Deployment

1. Go to the **Actions** tab in your repository
2. You should see a workflow run called "Deploy to GitHub Pages"
3. Wait for it to complete (usually takes 1-2 minutes)
4. Once complete, you'll see a green checkmark

### Step 5: Access Your Site

Your site will be available at:
**https://visualGravitySense.github.io/punk_hacker_transformation/**

> Note: It may take a few minutes for the site to be accessible after the first deployment.

## 🔄 Automatic Deployment

Every time you push changes to the `main` branch, GitHub Actions will automatically:
1. Build your site
2. Deploy it to GitHub Pages
3. Make it available at the URL above

## 🐛 Troubleshooting

### Site not loading?
- Check the **Actions** tab for any errors
- Verify that GitHub Pages is enabled in Settings
- Wait a few minutes and try again (first deployment can take up to 10 minutes)

### Workflow failing?
- Make sure the workflow file (`.github/workflows/deploy.yml`) is in the repository
- Check that you have write permissions to the repository
- Verify that GitHub Pages is enabled

## 📝 Manual Deployment

If you prefer to deploy manually:

1. Go to **Settings** → **Pages**
2. Under **Source**, select **GitHub Actions**
3. The workflow will run automatically on the next push

---

**Need help?** Open an issue in the repository!

