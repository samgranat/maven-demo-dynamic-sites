# GitHub Setup Instructions

Follow these steps to push this repository to GitHub.

## Option 1: Using GitHub Desktop (Easiest)

1. **Download GitHub Desktop** (if not installed)
   - Visit: https://desktop.github.com/
   - Install and sign in with your GitHub account

2. **Add this repository**
   - Open GitHub Desktop
   - Click: `File` → `Add Local Repository`
   - Browse to: `/Users/samgranat/magi-demo/maven-demos-repo`
   - Click: `Add Repository`

3. **Publish to GitHub**
   - Click: `Publish repository` button (top right)
   - Enter repository name: `maven-demos` (or your preferred name)
   - Choose: Public or Private
   - Click: `Publish Repository`

4. **Done!** Your demos are now on GitHub.

## Option 2: Using Command Line

### Step 1: Create a new repository on GitHub

1. Go to: https://github.com/new
2. Repository name: `maven-demos`
3. Description: "Maven AI demo sites for Travel, Telecom, Financial, and B2B verticals"
4. Choose: Public or Private
5. **DO NOT** initialize with README (we already have one)
6. Click: `Create repository`

### Step 2: Push your local repository

```bash
cd /Users/samgranat/magi-demo/maven-demos-repo

# Add GitHub as remote (replace YOUR-USERNAME with your GitHub username)
git remote add origin https://github.com/YOUR-USERNAME/maven-demos.git

# Push to GitHub
git branch -M main
git push -u origin main
```

### Step 3: Verify

Visit: `https://github.com/YOUR-USERNAME/maven-demos`

You should see all your demos!

## Option 3: Using GitHub CLI (if installed)

```bash
cd /Users/samgranat/magi-demo/maven-demos-repo

# Create repo and push (public)
gh repo create maven-demos --public --source=. --push

# OR create private repo
gh repo create maven-demos --private --source=. --push
```

## What Gets Pushed

```
maven-demos/
├── README.md (main documentation)
├── .gitignore (excludes system files)
├── travel-aventra/ (Aventra travel demo)
├── telecom-televia/ (Televia telecom demo)
├── financial-flowfi/ (FlowFi financial demo)
└── b2b-kikkocrm/ (KikkoCRM B2B demo)
```

## After Pushing to GitHub

### Enable GitHub Pages (Optional)

You can host the demos directly on GitHub:

1. Go to your repo settings
2. Navigate to: `Settings` → `Pages`
3. Source: `Deploy from a branch`
4. Branch: `main` → folder: `/travel-aventra` (or any demo)
5. Click: `Save`

Your demo will be live at:
`https://YOUR-USERNAME.github.io/maven-demos/`

### Share the Repository

Share your GitHub URL with engineers:
```
https://github.com/YOUR-USERNAME/maven-demos
```

They can:
- Clone the repo: `git clone https://github.com/YOUR-USERNAME/maven-demos.git`
- View files online
- Download as ZIP
- Fork and customize

## Making Updates

After you make changes locally:

```bash
cd /Users/samgranat/magi-demo/maven-demos-repo
git add .
git commit -m "Update travel demo styling"
git push
```

## Troubleshooting

### Authentication Error

If you get authentication errors:

1. **Use Personal Access Token** (recommended)
   - Go to: https://github.com/settings/tokens
   - Generate new token (classic)
   - Select scopes: `repo`
   - Copy token
   - Use token as password when pushing

2. **Or use SSH**
   - Set up SSH keys: https://docs.github.com/en/authentication/connecting-to-github-with-ssh

### Already Exists Error

If the repo name is taken:
```bash
git remote set-url origin https://github.com/YOUR-USERNAME/NEW-REPO-NAME.git
```

## Next Steps

After pushing to GitHub:
1. Update the README with your live URLs
2. Add screenshots to the repo
3. Enable GitHub Pages for live hosting
4. Share the repo URL with your team

---

**Need help?** GitHub Docs: https://docs.github.com/
