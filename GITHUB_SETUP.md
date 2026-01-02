# GitHub Pages Setup - Step by Step

Follow these steps to deploy your meditation app to GitHub Pages:

## Step 1: Create GitHub Repository

1. Go to https://github.com/new
2. Repository name: `meditation-app` (or any name you like)
3. Make sure it's set to **Public** (required for free GitHub Pages)
4. **Don't** initialize with README, .gitignore, or license
5. Click **"Create repository"**

## Step 2: Open Terminal and Navigate to Your Project

Open Terminal and run:

```bash
cd "/Users/jessicali/meditation app"
```

## Step 3: Initialize Git and Push to GitHub

Copy and paste these commands one by one (replace `YOUR_USERNAME` with your GitHub username):

```bash
# Initialize git repository
git init

# Add all files
git add .

# Make your first commit
git commit -m "Initial commit: Meditation app"

# Add your GitHub repository (replace YOUR_USERNAME with your actual GitHub username)
git remote add origin https://github.com/YOUR_USERNAME/meditation-app.git

# Rename branch to main (if needed)
git branch -M main

# Push to GitHub
git push -u origin main
```

**Note:** When you run `git push`, GitHub will ask for your username and password. 
- **Username:** Your GitHub username
- **Password:** Use a **Personal Access Token** (not your GitHub password)

### How to Create a Personal Access Token:

1. Go to: https://github.com/settings/tokens
2. Click **"Generate new token"** → **"Generate new token (classic)"**
3. Name it: "Meditation App"
4. Check the **"repo"** scope
5. Click **"Generate token"**
6. **Copy the token** (you won't see it again!)
7. Use this token as your password when pushing

## Step 4: Enable GitHub Pages

1. Go to your repository on GitHub: `https://github.com/YOUR_USERNAME/meditation-app`
2. Click the **Settings** tab
3. Scroll down to **Pages** in the left sidebar
4. Under **Source**, select:
   - Branch: **main**
   - Folder: **/ (root)**
5. Click **Save**
6. Wait 1-2 minutes for GitHub to build your site

## Step 5: Access Your App

Your app will be available at:
```
https://YOUR_USERNAME.github.io/meditation-app/
```

## Step 6: Add to Phone Home Screen

### iPhone:
1. Open the URL in Safari
2. Tap Share button (square with arrow)
3. Tap "Add to Home Screen"
4. Name it "Just Breathe"
5. Tap "Add"

### Android:
1. Open the URL in Chrome
2. Tap menu (3 dots)
3. Tap "Add to Home Screen" or "Install App"
4. Name it "Just Breathe"
5. Tap "Add"

## Troubleshooting

**If git push fails:**
- Make sure you're using a Personal Access Token, not your password
- Check that the repository name matches exactly
- Verify the repository is set to Public

**If Pages doesn't work:**
- Make sure the repository is Public
- Wait a few minutes for GitHub to process
- Check that `index.html` is in the root folder

**Need help?** The repository should have:
- `index.html` (your app)
- `README.md`
- `.gitignore`

That's it! Your meditation app is now live on the web! 🎉

