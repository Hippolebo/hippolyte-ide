# GitHub Pages Setup Guide

## Files Created for Your Website

✅ **Main Pages:**
- `index.md` - Homepage for the research project
- `README.md` - GitHub repository description
- `belgium/index.md` - Belgium analysis page

✅ **Configuration:**
- `_config.yml` - GitHub Pages theme and settings
- `.gitignore` - Excludes unnecessary files from Git

✅ **Data:**
- `belgium/data/belgian_stocks_filtered_sorted.csv` - Downloadable data

---

## Quick Start: Push to GitHub

### Step 1: Initialize Git (Run these commands in Terminal)

```bash
cd "/Users/hippolyteide/Documents/maastricht/projects/research project"

# Initialize git repository
git init

# Add all files
git add .

# Create first commit
git commit -m "Initial commit: Low P/E Europe research project with Belgium analysis"
```

### Step 2: Connect to GitHub

**Option A: New Repository (if you haven't created it yet)**

```bash
# Create a new repository on GitHub first, then:
git remote add origin https://github.com/YOUR_USERNAME/hippolyte-ide.git
git branch -M main
git push -u origin main
```

**Option B: Add to Existing Repository**

If you already have a repository called `hippolyte-ide`, you have two options:

**Option B1: Create as a subdirectory/project folder**
```bash
# Clone your existing repository
cd ~/Documents/maastricht/projects
git clone https://github.com/YOUR_USERNAME/hippolyte-ide.git

# Copy your research project into it
cp -r "research project" hippolyte-ide/low-pe-europe/

# Commit and push
cd hippolyte-ide
git add low-pe-europe/
git commit -m "Add Low P/E Europe research project"
git push origin main
```

**Option B2: Create as a separate repository**
```bash
# In the research project directory
git remote add origin https://github.com/YOUR_USERNAME/low-pe-europe.git
git branch -M main
git push -u origin main
```

---

## Step 3: Enable GitHub Pages

1. Go to your repository on GitHub
2. Click **Settings**
3. Scroll down to **Pages** (in the left sidebar)
4. Under **Source**, select:
   - Branch: `main`
   - Folder: `/ (root)`
5. Click **Save**

**Your site will be live at:**
- `https://YOUR_USERNAME.github.io/hippolyte-ide/` (if subdirectory)
- `https://YOUR_USERNAME.github.io/low-pe-europe/` (if separate repo)

---

## Step 4: Test Your Site

Wait 1-2 minutes for GitHub to build your site, then visit your URL!

---

## Recommended Structure for Portfolio Site

If `hippolyte-ide` is your main portfolio site:

```
hippolyte-ide/
├── index.html or index.md       (Your main portfolio homepage)
├── projects/
│   ├── low-pe-europe/            (This research project)
│   │   ├── index.md
│   │   ├── belgium/
│   │   └── ...
│   ├── other-project-1/
│   └── other-project-2/
└── about.md
```

Then link to it from your main portfolio page:
```markdown
## Projects
- [Low P/E Europe Research](projects/low-pe-europe/) - Value investing analysis
```

---

## Future Updates

When you add new countries (France, Germany, etc.):

```bash
# Make your changes (add new files)

# Stage changes
git add .

# Commit
git commit -m "Add France analysis"

# Push to GitHub
git push origin main
```

GitHub Pages will automatically rebuild your site!

---

## Changing the Theme

Edit `_config.yml` and change the `theme:` line to one of these:

- `minima` (default, clean)
- `jekyll-theme-cayman` (modern, professional)
- `jekyll-theme-minimal` (simple, minimal)
- `jekyll-theme-slate` (dark theme)

Commit and push to see the change!

---

## Next Steps

1. ✅ Push to GitHub (follow Step 1-2 above)
2. ✅ Enable GitHub Pages (Step 3)
3. ✅ Share your site URL on X
4. 🔄 Add France analysis next
5. 🔄 Update performance quarterly

---

## Need Help?

- **GitHub Pages docs:** https://docs.github.com/en/pages
- **Jekyll themes:** https://pages.github.com/themes/
- **Markdown guide:** https://guides.github.com/features/mastering-markdown/

---

Good luck! 🚀
