# GitHub Deployment Guide

Your code is ready to be pushed to GitHub! Follow these steps:

## Step 1: Create a GitHub Repository

1. Go to [GitHub.com](https://github.com) and sign in
2. Click the **"+"** icon in the top right corner
3. Select **"New repository"**
4. Fill in the details:
   - **Repository name**: `study-tracker` (or any name you prefer)
   - **Description**: "BDA Study Progress Tracker - Real-time study time management tool"
   - **Visibility**: Choose Public or Private
   - **DO NOT** initialize with README, .gitignore, or license (we already have these)
5. Click **"Create repository"**

## Step 2: Connect and Push Your Code

After creating the repository, GitHub will show you commands. Use these commands in your terminal:

```powershell
# Navigate to your project (if not already there)
cd "D:\Projects\Study Tracker"

# Add the remote repository (replace YOUR_USERNAME with your GitHub username)
git remote add origin https://github.com/YOUR_USERNAME/study-tracker.git

# Rename branch to main (if needed)
git branch -M main

# Push your code
git push -u origin main
```

## Step 3: Deploy to GitHub Pages (Optional - Free Hosting)

1. Go to your repository on GitHub
2. Click on **"Settings"** tab
3. Scroll down to **"Pages"** in the left sidebar
4. Under **"Source"**, select **"Deploy from a branch"**
5. Choose **"main"** branch and **"/ (root)"** folder
6. Click **"Save"**
7. Your site will be live at: `https://YOUR_USERNAME.github.io/study-tracker/`

## Alternative: Quick Deploy Commands

If you want to do it all from command line, you can use:

```powershell
# Set your GitHub username and repo name
$GITHUB_USER = "YOUR_USERNAME"
$REPO_NAME = "study-tracker"

# Add remote
git remote add origin https://github.com/$GITHUB_USER/$REPO_NAME.git

# Push
git branch -M main
git push -u origin main
```

## Troubleshooting

- **Authentication required**: You may need to use a Personal Access Token instead of password
- **Repository already exists**: Make sure the repo name is unique or use a different name
- **Permission denied**: Check that you're logged into GitHub and have permission to create repos

