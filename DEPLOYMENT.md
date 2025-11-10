# Deployment Instructions for GitHub Pages

Your personal website is ready to be deployed! Follow these steps to host it on GitHub Pages.

## Option 1: Using GitHub Website (Recommended)

### Step 1: Create a GitHub Repository

1. Go to [GitHub](https://github.com) and log in to your account
2. Click the **+** icon in the top-right corner and select **New repository**
3. Fill in the repository details:
   - **Repository name**: `personal-website` (or any name you prefer)
   - **Description**: "Personal academic website showcasing my research and projects"
   - **Visibility**: Public (required for free GitHub Pages)
   - **Do NOT** initialize with README, .gitignore, or license (we already have these)
4. Click **Create repository**

### Step 2: Push Your Code to GitHub

After creating the repository, GitHub will show you some commands. Run these in your terminal:

```bash
cd /home/rgbsm/resume/website
git remote add origin https://github.com/marati-bhaskar/personal-website.git
git push -u origin main
```

**Note**: Replace `marati-bhaskar` with your actual GitHub username if different, and `personal-website` with your repository name if you chose a different name.

If prompted for credentials:
- **Username**: Your GitHub username
- **Password**: Use a Personal Access Token (not your GitHub password)
  - To create a token: Go to GitHub → Settings → Developer settings → Personal access tokens → Generate new token
  - Select scopes: `repo` (full control of private repositories)
  - Copy the token and use it as your password

### Step 3: Enable GitHub Pages

1. Go to your repository on GitHub
2. Click on **Settings** (gear icon in the repository navigation)
3. In the left sidebar, click on **Pages**
4. Under **Source**:
   - Select branch: `main`
   - Select folder: `/ (root)`
5. Click **Save**

### Step 4: Access Your Website

After a few minutes, your website will be live at:
```
https://marati-bhaskar.github.io/personal-website/
```

GitHub will show you the URL on the Pages settings page.

---

## Option 2: Using GitHub CLI (Advanced)

If you have GitHub CLI installed and authenticated:

```bash
cd /home/rgbsm/resume/website

# Create repository
gh repo create personal-website --public --source=. --remote=origin --push

# Enable GitHub Pages
gh api repos/marati-bhaskar/personal-website/pages \
  -X POST \
  -F source[branch]=main \
  -F source[path]=/
```

---

## Updating Your Website

After making changes to your website:

```bash
cd /home/rgbsm/resume/website
git add .
git commit -m "Description of your changes"
git push
```

Your changes will be live within 1-2 minutes!

---

## Custom Domain (Optional)

To use a custom domain like `www.yourdomain.com`:

1. Buy a domain from a registrar (e.g., Namecheap, Google Domains, GoDaddy)
2. Add a `CNAME` file in your repository root with your domain:
   ```bash
   echo "www.yourdomain.com" > CNAME
   git add CNAME
   git commit -m "Add custom domain"
   git push
   ```
3. In your domain registrar's DNS settings, add:
   - Type: `CNAME`
   - Host: `www`
   - Value: `marati-bhaskar.github.io`
4. In GitHub repository settings → Pages, add your custom domain

---

## Troubleshooting

### Issue: 404 Error

**Solution**: 
- Ensure GitHub Pages is enabled in repository settings
- Wait 5-10 minutes after enabling Pages
- Check that your repository is public
- Verify the branch name is correct

### Issue: Changes Not Showing

**Solution**:
- Clear your browser cache (Ctrl+Shift+R or Cmd+Shift+R)
- Wait a few minutes for GitHub to rebuild the site
- Check that your changes were pushed: `git log` and `git status`

### Issue: Authentication Failed

**Solution**:
- Use a Personal Access Token instead of password
- Generate token: GitHub → Settings → Developer settings → Personal access tokens
- Configure Git to use token:
  ```bash
  git config --global credential.helper cache
  ```

---

## Repository Status

✅ Local repository initialized  
✅ Files committed to git  
⏳ Waiting for GitHub repository creation  
⏳ Waiting for push to GitHub  
⏳ Waiting for GitHub Pages configuration  

---

## Quick Reference

| Action | Command |
|--------|---------|
| Check status | `git status` |
| See commit history | `git log --oneline` |
| Undo changes | `git checkout -- <file>` |
| Create new branch | `git checkout -b <branch-name>` |
| View remote URL | `git remote -v` |

---

## Need Help?

- [GitHub Pages Documentation](https://docs.github.com/en/pages)
- [Git Documentation](https://git-scm.com/doc)
- Contact: cs24d001@iittp.ac.in

---

**Your website files are ready at**: `/home/rgbsm/resume/website/`

**Next Step**: Follow Option 1 above to create the GitHub repository and deploy your website! 🚀

