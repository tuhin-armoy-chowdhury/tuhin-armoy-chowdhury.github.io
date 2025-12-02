# How to Upload and Host Your Portfolio on GitHub

## Step 1: Create a GitHub Repository

1. Go to [GitHub.com](https://github.com) and sign in
2. Click the **"+"** icon in the top right corner
3. Select **"New repository"**
4. Repository name: `portfolio` (or any name you prefer)
5. Description: "My personal portfolio website"
6. Make it **Public** (required for free GitHub Pages)
7. **DO NOT** initialize with README, .gitignore, or license (we already have files)
8. Click **"Create repository"**

## Step 2: Upload Files Using Git (Terminal Commands)

Open your terminal in the project folder and run these commands:

```bash
# Navigate to your project folder
cd "/home/tuhin/Downloads/My Minimal Portfolio"

# Initialize git repository
git init

# Add all files
git add .

# Create initial commit
git commit -m "Initial commit: Portfolio website"

# Add your GitHub repository as remote (replace YOUR_USERNAME with your GitHub username)
git remote add origin https://github.com/YOUR_USERNAME/portfolio.git

# Push to GitHub
git branch -M main
git push -u origin main
```

**Note:** You'll be prompted for your GitHub username and password (or personal access token).

## Step 3: Enable GitHub Pages

1. Go to your repository on GitHub
2. Click on **"Settings"** tab
3. Scroll down to **"Pages"** in the left sidebar
4. Under **"Source"**, select **"Deploy from a branch"**
5. Choose **"main"** branch and **"/ (root)"** folder
6. Click **"Save"**

## Step 4: Access Your Live Website

Your portfolio will be available at:
```
https://YOUR_USERNAME.github.io/portfolio/
```

It may take a few minutes for the site to go live after enabling GitHub Pages.

## Alternative: Using GitHub Desktop (GUI Method)

If you prefer a graphical interface:

1. Download [GitHub Desktop](https://desktop.github.com/)
2. Sign in with your GitHub account
3. Click **"File" → "Add Local Repository"**
4. Select your project folder
5. Click **"Publish repository"** in GitHub Desktop
6. Follow the prompts to create the repository on GitHub
7. Enable GitHub Pages as described in Step 3 above

## Updating Your Portfolio

Whenever you make changes:

```bash
git add .
git commit -m "Description of your changes"
git push
```

Your GitHub Pages site will automatically update within a few minutes.

