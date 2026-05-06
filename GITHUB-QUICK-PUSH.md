# 🚀 Quick GitHub Push Commands
**Copy-paste ready for PowerShell**

---

## ⚡ Fast Track (5 Commands)

```powershell
# 1. Initialize Git (if not already done)
git init
git branch -M main

# 2. Add all files
git add .

# 3. Commit
git commit -m "Initial commit: Faheem Akbar Portfolio - Production ready"

# 4. Add GitHub remote (replace YOUR_USERNAME)
git remote add origin https://github.com/YOUR_USERNAME/faheem-akbar-portfolio.git

# 5. Push to GitHub
git push -u origin main
```

**That's it!** Your portfolio is now on GitHub. ✅

---

## 🔍 Verify Before Push

```powershell
# Check what will be committed
git status

# See ignored files (should NOT commit these)
# node_modules/, dist/, backup_*/ should be listed
git status --ignored
```

---

## 📝 Common Follow-up Commands

### After making changes:
```powershell
git add .
git commit -m "Your change description"
git push
```

### Create new branch:
```powershell
git checkout -b feature-name
git push -u origin feature-name
```

### Check repository status:
```powershell
git status
git log --oneline -5
```

---

## ✅ What Gets Committed

**Included (Safe):**
- ✅ HTML, CSS, JavaScript files
- ✅ .htaccess (security config)
- ✅ package.json (dependencies)
- ✅ All .md documentation
- ✅ build-scripts/
- ✅ js/ folder (all files safe)

**Excluded (Via .gitignore):**
- ❌ node_modules/
- ❌ dist/ (build output)
- ❌ backup_*/ folders
- ❌ .env files (if created)

---

## 🌐 Enable GitHub Pages

After push, enable hosting:

```powershell
# Using GitHub CLI (if installed)
gh repo edit --enable-pages --pages-branch main

# Or manually:
# 1. Go to: https://github.com/YOUR_USERNAME/faheem-akbar-portfolio/settings/pages
# 2. Source: main branch, /root
# 3. Save
```

**Live URL:**
```
https://YOUR_USERNAME.github.io/faheem-akbar-portfolio/
```

---

## 🔒 Security Reminder

**Your files are safe to commit!**
- No API keys or secrets in your code
- Sentry DSN is public by design
- All frontend code is meant to be visible
- .gitignore protects sensitive files

**Push with confidence!** 🎯
