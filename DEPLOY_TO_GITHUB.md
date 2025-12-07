# 🚀 Deploy EduTrack to GitHub Pages

This guide will walk you through deploying your Attendance System to GitHub Pages so it's accessible online for free.

## Prerequisites

- A GitHub account ([Sign up here](https://github.com/join))
- Git installed on your computer ([Download here](https://git-scm.com/downloads))
- Your Attendance System files

## Step-by-Step Deployment

### 1. Create a GitHub Repository

1. Go to [GitHub](https://github.com) and sign in
2. Click the **"+"** icon in the top-right corner
3. Select **"New repository"**
4. Fill in the details:
   - **Repository name**: `Attendance-System-New` (or any name you prefer)
   - **Description**: "Modern attendance tracking system"
   - **Public** or **Private**: Choose Public for GitHub Pages
   - Don't initialize with README (we already have one)
5. Click **"Create repository"**

### 2. Initialize Git in Your Project

Open a terminal/command prompt in your project folder and run:

```bash
# Navigate to your project folder
cd "c:\xampp\htdocs\Attendance System"

# Initialize Git repository
git init

# Add all files
git add .

# Commit the files
git commit -m "Initial commit: EduTrack Attendance System"
```

### 3. Connect to GitHub and Push

Replace `YOUR_USERNAME` and `REPOSITORY_NAME` with your actual GitHub username and repository name:

```bash
# Add GitHub repository as remote
git remote add origin https://github.com/YOUR_USERNAME/REPOSITORY_NAME.git

# Rename branch to main (if needed)
git branch -M main

# Push to GitHub
git push -u origin main
```

**Note:** You may be prompted to sign in to GitHub. Use your GitHub credentials.

### 4. Enable GitHub Pages

1. Go to your repository on GitHub
2. Click on **"Settings"** tab
3. Scroll down to **"Pages"** in the left sidebar
4. Under **"Source"**, select:
   - **Branch**: `main`
   - **Folder**: `/ (root)`
5. Click **"Save"**

### 5. Access Your Live Site

After a few minutes, your site will be live at:

```
https://YOUR_USERNAME.github.io/REPOSITORY_NAME/
```

For example: `https://sora99999.github.io/Attendance-System-New/`

## 🎉 You're Done!

Your Attendance System is now live and accessible online!

## Updating Your Site

Whenever you make changes to your code:

```bash
# Add changes
git add .

# Commit changes
git commit -m "Description of your changes"

# Push to GitHub
git push
```

GitHub Pages will automatically update within a few minutes.

## Troubleshooting

### Site Not Loading?
- Wait 5-10 minutes after enabling Pages
- Check that you selected the correct branch and folder
- Ensure your repository is Public (or you have GitHub Pro for private Pages)

### Broken Images/Links?
- Make sure all file paths are relative (not absolute)
- Check that file names match exactly (case-sensitive)

### Data Not Saving?
- This is normal! The system uses localStorage which is browser-specific
- Each user will have their own data on their device
- Export to Excel regularly as backup

## Custom Domain (Optional)

Want to use your own domain like `attendance.yourdomain.com`?

1. Buy a domain from a registrar (Namecheap, GoDaddy, etc.)
2. In your repository settings under Pages, add your custom domain
3. Configure DNS records at your domain registrar
4. Follow [GitHub's custom domain guide](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site)

## Need Help?

- [GitHub Pages Documentation](https://docs.github.com/en/pages)
- [Git Basics Guide](https://git-scm.com/book/en/v2/Getting-Started-Git-Basics)
- GitHub Community Forum

---

**Happy Teaching! 📚✨**
