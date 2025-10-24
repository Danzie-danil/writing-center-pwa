# SIMPLE DEPLOYMENT INSTRUCTIONS

## YOUR INFORMATION (Already Configured)
- Email: danielidrissa12@gmail.com
- Username: Danzie-danil
- Repository: writing-center-pwa
- Live URL: https://danzie-danil.github.io/writing-center-pwa/

All files are already configured with correct paths!

---

## STEP 1: One-Time Git Setup

Open Git Bash and run these TWO commands:

```bash
git config --global user.email "danielidrissa12@gmail.com"
git config --global user.name "Danzie-danil"
```

That's it! You only need to do this once ever.

---

## STEP 2: Replace Your Old Files

1. Delete everything in: `C:\Users\User\Desktop\writing-center-pwa`
2. Copy ALL files from this fresh download into that folder
3. Make sure the `icons` folder is also copied

Your folder should now contain:
- index.html
- manifest.json
- service-worker.js
- icons/ (folder with 8 PNG files)
- DEPLOY_INSTRUCTIONS.md (this file)

---

## STEP 3: Open Git Bash in Your Folder

1. Open File Explorer
2. Go to: `C:\Users\User\Desktop\writing-center-pwa`
3. Right-click in the empty space (not on a file)
4. Click "Git Bash Here"

---

## STEP 4: Run These Commands

Copy and paste these commands ONE AT A TIME into Git Bash:

### Initialize Git (if needed)
```bash
git init
```

### Add all files
```bash
git add .
```

### Commit files
```bash
git commit -m "Fresh PWA deployment with correct paths"
```

### Set branch to main
```bash
git branch -M main
```

### Add your GitHub repository
```bash
git remote remove origin
git remote add origin https://github.com/Danzie-danil/writing-center-pwa.git
```

### Push to GitHub
```bash
git push -u origin main --force
```

Note: We use `--force` because we're replacing everything with fresh files.

---

## STEP 5: Wait and Test

1. Wait 2-3 minutes for GitHub to rebuild your site
2. Visit: https://danzie-danil.github.io/writing-center-pwa/
3. Press Ctrl+Shift+R to hard refresh
4. The site should load perfectly!
5. Look for the "Install App" button

---

## IF YOU GET AN ERROR

### "Authentication failed"
You need a Personal Access Token instead of your password:

1. Go to: https://github.com/settings/tokens
2. Click "Generate new token (classic)"
3. Give it a name: "Writing Center"
4. Check the "repo" checkbox
5. Click "Generate token"
6. Copy the token
7. Use it as your password when Git asks

### "fatal: not a git repository"
Make sure you're in the correct folder. Run:
```bash
pwd
```
It should show: `/c/Users/User/Desktop/writing-center-pwa`

### Other errors
1. Make sure Git Bash is open in the correct folder
2. Make sure you ran the git config commands in STEP 1
3. Try closing Git Bash and opening it again

---

## THAT'S IT!

After `git push` succeeds:
- Your site updates automatically
- Wait 2-3 minutes
- Refresh the page
- Everything should work!

All paths are already correct for your subdirectory deployment.

---

## Future Updates

To update your site later:

```bash
# Make your changes to files, then:
git add .
git commit -m "Description of your changes"
git push
```

---

Made for: Danzie-danil
Repository: https://github.com/Danzie-danil/writing-center-pwa
Live Site: https://danzie-danil.github.io/writing-center-pwa/
