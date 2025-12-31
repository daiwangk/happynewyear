# Deploy to Vercel - Step by Step Guide

## Method 1: Drag & Drop (Easiest - No Installation Needed)

1. Go to https://vercel.com and sign in (or create an account)
2. In your dashboard, click **"Add New..."** → **"Project"**
3. Click **"Browse"** or drag and drop your `new_year` folder
4. Vercel will automatically detect your static HTML file
5. Click **"Deploy"** - that's it!
6. Your site will be live at a URL like: `https://new-year-xxxxx.vercel.app`

## Method 2: Using Vercel CLI

### Step 1: Install Vercel CLI
```bash
npm install -g vercel
```

### Step 2: Login to Vercel
```bash
vercel login
```

### Step 3: Deploy
```bash
vercel
```

Follow the prompts:
- Set up and deploy? **Yes**
- Which scope? (select your account)
- Link to existing project? **No**
- What's your project's name? (press Enter for default: `new_year`)
- In which directory is your code located? (press Enter for `./`)

### Step 4: Production Deploy
```bash
vercel --prod
```

Your site will be live at: `https://new-year.vercel.app` (or your chosen domain)

## Method 3: Using Git (GitHub/GitLab/Bitbucket)

### Step 1: Initialize Git (if not already done)
```bash
git init
git add .
git commit -m "Initial commit"
```

### Step 2: Push to GitHub
1. Create a new repository on GitHub
2. Push your code:
```bash
git remote add origin <your-github-repo-url>
git branch -M main
git push -u origin main
```

### Step 3: Connect to Vercel
1. Go to https://vercel.com
2. Click **"Add New..."** → **"Project"**
3. Import your GitHub repository
4. Click **"Deploy"**
5. Future pushes to your repo will automatically deploy!

---

## Important Notes:

- Your `index.html` file is already in the correct location (root directory)
- Vercel automatically serves `index.html` as the default page
- No additional configuration is needed for a static HTML site
- Vercel provides free SSL certificates automatically
- Your site will be live on a `*.vercel.app` domain

## After Deployment:

You can:
- View your site at the provided URL
- Customize the domain in Vercel dashboard
- Set up automatic deployments (if using Git)
- Monitor analytics and performance

---

**Recommended:** Use **Method 1 (Drag & Drop)** if you want the fastest deployment without any setup!

