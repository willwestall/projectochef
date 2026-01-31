# Deployment Guide for Projecto Chef

This guide will walk you through deploying your Projecto Chef website to Vercel with GitHub integration.

## 📋 Prerequisites

- A GitHub account (free) - [Sign up here](https://github.com/join)
- A Vercel account (free) - [Sign up here](https://vercel.com/signup)
- Your project files ready to upload

## 🚀 Step 1: Upload to GitHub

### Option A: Using GitHub Website (Easiest for Beginners)

1. **Create a new repository:**
   - Go to [github.com](https://github.com) and log in
   - Click the **"+"** button in top right → **"New repository"**
   - Repository name: `projectochef` (or whatever you prefer)
   - Description: "Cookbook projector for kitchen counters"
   - Choose **Public** (required for free Vercel hosting)
   - ✅ Check "Add a README file"
   - Click **"Create repository"**

2. **Upload your files:**
   - Click **"Add file"** → **"Upload files"**
   - Drag and drop these files:
     - `index.html`
     - `.gitignore`
   - Scroll down and click **"Commit changes"**

### Option B: Using Git Command Line

```bash
# Navigate to your project folder
cd /path/to/your/project

# Initialize Git
git init

# Add all files
git add .

# Commit
git commit -m "Initial commit - Projecto Chef website"

# Add your GitHub repository as remote
git remote add origin https://github.com/YOUR-USERNAME/projectochef.git

# Push to GitHub
git branch -M main
git push -u origin main
```

## 🌐 Step 2: Deploy to Vercel

1. **Go to Vercel:**
   - Visit [vercel.com](https://vercel.com)
   - Click **"Sign Up"** (or **"Login"** if you have an account)

2. **Sign up with GitHub:**
   - Click **"Continue with GitHub"**
   - Authorize Vercel to access your GitHub account

3. **Import your project:**
   - Click **"Add New..."** → **"Project"**
   - Find `projectochef` in your repository list
   - Click **"Import"**

4. **Configure project:**
   - **Project Name:** `projectochef` (or customize)
   - **Framework Preset:** Leave as "Other"
   - **Root Directory:** `./`
   - **Build Command:** Leave empty (not needed for HTML)
   - **Output Directory:** Leave empty
   - Click **"Deploy"**

5. **Wait for deployment:**
   - Vercel will deploy your site (takes ~30 seconds)
   - You'll get a URL like `projectochef.vercel.app`
   - Click **"Visit"** to see your live site! 🎉

## 🔄 Step 3: Auto-Deployments (Already Set Up!)

Good news! Auto-deployments are automatically enabled when you connect GitHub to Vercel.

**How it works:**
- Every time you push changes to your `main` branch on GitHub
- Vercel automatically rebuilds and redeploys your site
- Changes go live in ~30 seconds

**To update your website:**
1. Edit your files locally
2. Upload to GitHub (use "Upload files" or git commands)
3. Vercel automatically deploys the changes
4. Your site updates automatically!

## 🎨 Step 4: Custom Domain (Optional)

Want `projectochef.com` instead of `projectochef.vercel.app`?

1. **Buy a domain** (~$10-15/year):
   - [Namecheap.com](https://namecheap.com)
   - [Google Domains](https://domains.google)
   - [Porkbun.com](https://porkbun.com)

2. **Connect to Vercel:**
   - In Vercel dashboard, go to your project
   - Click **"Settings"** → **"Domains"**
   - Enter your domain name
   - Follow the instructions to update DNS settings
   - Wait 24-48 hours for DNS to propagate

## 🛠️ Making Updates

### Using GitHub Website:
1. Go to your repository on GitHub
2. Click on `index.html`
3. Click the **pencil icon** (Edit)
4. Make your changes
5. Scroll down and click **"Commit changes"**
6. Vercel automatically deploys in ~30 seconds!

### Using Git Commands:
```bash
# Make your changes to index.html

# Stage changes
git add index.html

# Commit
git commit -m "Updated website content"

# Push to GitHub
git push

# Vercel automatically deploys!
```

## ✅ Verification Checklist

After deployment, verify:
- [ ] Website loads at your Vercel URL
- [ ] All 4 pages work (Home, Shop, About, Contact)
- [ ] Navigation tabs switch between pages
- [ ] Hamburger menu works on mobile
- [ ] Email popup appears after 15 seconds
- [ ] Contact form shows confirmation
- [ ] Buy button shows alert
- [ ] All text is readable and properly formatted

## 🐛 Troubleshooting

**Site not loading?**
- Check that `index.html` is in the root directory of your repo
- Make sure repository is Public (not Private)

**Changes not appearing?**
- Check Vercel dashboard for deployment status
- May take up to 1 minute for changes to appear
- Try hard refresh: `Ctrl + Shift + R` (Windows) or `Cmd + Shift + R` (Mac)

**404 Error?**
- Ensure file is named exactly `index.html` (lowercase)
- Check that file is in root directory, not a subfolder

## 📞 Need Help?

- **Vercel Documentation:** [vercel.com/docs](https://vercel.com/docs)
- **GitHub Documentation:** [docs.github.com](https://docs.github.com)
- **Vercel Discord:** [vercel.com/discord](https://vercel.com/discord)

---

**Congratulations! Your Projecto Chef website is now live! 🎉**
