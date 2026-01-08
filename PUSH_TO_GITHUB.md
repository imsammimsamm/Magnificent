# Step-by-Step Guide: Pushing to GitHub

## Step 1: Open Terminal

**On Mac:**
- Press `Command + Space` to open Spotlight
- Type "Terminal" and press Enter
- OR go to Applications → Utilities → Terminal

## Step 2: Navigate to Your Deploy Folder

Copy and paste this command into Terminal:

```bash
cd /Users/aayush/Downloads/MagDia-Website-main/deploy
```

**What this does:** Changes your current directory to the deploy folder where your website files are.

**Press Enter** after typing the command.

## Step 3: Verify You're in the Right Place

Type this command to see your files:

```bash
ls
```

**What this does:** Lists all files in the current folder. You should see:
- index.html
- README.md
- images/
- static/
- etc.

## Step 4: Add Your GitHub Repository as Remote

**First, get your repository URL from GitHub:**
1. Go to your GitHub repository page
2. Click the green "Code" button
3. Copy the HTTPS URL (it looks like: `https://github.com/yourusername/repo-name.git`)

**Then run this command (replace with YOUR repository URL):**

```bash
git remote add origin https://github.com/YOUR-USERNAME/YOUR-REPO-NAME.git
```

**Example:**
```bash
git remote add origin https://github.com/aayush/magnificent-diamond-website.git
```

**What this does:** Tells git where to push your code (your GitHub repository).

**Press Enter** after typing the command.

## Step 5: Set the Branch Name to "main"

```bash
git branch -M main
```

**What this does:** Renames your branch to "main" (GitHub's default branch name).

**Press Enter** after typing the command.

## Step 6: Push Your Code to GitHub

```bash
git push -u origin main
```

**What this does:** Uploads all your files to GitHub.

**Press Enter** after typing the command.

**You may be asked to:**
- Enter your GitHub username
- Enter your GitHub password (or Personal Access Token)

## Step 7: Verify It Worked

1. Go to your GitHub repository page in your browser
2. Refresh the page
3. You should see all your files there!

## Troubleshooting

### If you get "remote origin already exists" error:
Run this first:
```bash
git remote remove origin
```
Then go back to Step 4.

### If you need to authenticate:
GitHub no longer accepts passwords. You'll need a Personal Access Token:
1. Go to GitHub.com → Settings → Developer settings → Personal access tokens → Tokens (classic)
2. Generate new token
3. Copy the token and use it as your password when pushing

### If you get permission errors:
Make sure you're using the correct repository URL and have access to it.
