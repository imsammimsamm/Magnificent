# Deployment Instructions

## Your website is ready for GitHub!

The repository has been initialized with:
- ✅ `index.html` in the root folder
- ✅ All assets in relative paths (`static/` and `images/` folders)
- ✅ Initial commit created
- ✅ README.md included

## Steps to Push to GitHub:

### Option 1: Create a New Repository on GitHub

1. Go to https://github.com/new
2. Create a new repository (e.g., `magnificent-diamond-website`)
3. **DO NOT** initialize with README, .gitignore, or license
4. Copy the repository URL (e.g., `https://github.com/yourusername/magnificent-diamond-website.git`)

5. Run these commands in the deploy folder:
```bash
cd /Users/aayush/Downloads/MagDia-Website-main/deploy
git remote add origin https://github.com/yourusername/magnificent-diamond-website.git
git branch -M main
git push -u origin main
```

### Option 2: Push to Existing Repository

If you already have a GitHub repository:

```bash
cd /Users/aayush/Downloads/MagDia-Website-main/deploy
git remote add origin https://github.com/yourusername/your-repo-name.git
git branch -M main
git push -u origin main
```

## Enable GitHub Pages:

1. Go to your repository on GitHub
2. Click **Settings** > **Pages**
3. Under "Source", select:
   - Branch: `main`
   - Folder: `/ (root)`
4. Click **Save**
5. Your site will be live at: `https://yourusername.github.io/repository-name`

## File Structure:

```
deploy/
├── index.html          (root - main entry point)
├── README.md
├── .gitignore
├── asset-manifest.json
├── images/            (all website images)
│   ├── logo.jpeg
│   ├── engagement-rings-diamond_og.webp
│   └── ...
└── static/           (CSS and JavaScript)
    ├── css/
    └── js/
```

All paths are configured to work from the root URL!
