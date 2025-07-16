# GitHub Setup Guide for Portfolio

## Quick Setup Steps

Since I cannot directly push to GitHub from this environment, here's how you can push your portfolio to your GitHub repository:

### Method 1: Using Replit's Git Integration (Recommended)

1. **In your Replit workspace:**
   - Click on the "Version Control" tab in the left sidebar
   - Click "Create a Git Repo" or "Connect to GitHub"
   - Authorize Replit to access your GitHub account

2. **Connect to your existing repository:**
   - Set remote URL: `https://github.com/Sanj-dot/Portfolio.git`
   - Add all files and commit with message: "Complete portfolio website with database integration"
   - Push to GitHub directly from Replit interface

### Method 2: Manual Git Commands

Run these commands in your Replit shell:

```bash
# Check current git status
git status

# Add your GitHub repository as remote (if not already added)
git remote add origin https://github.com/Sanj-dot/Portfolio.git

# Or update existing remote
git remote set-url origin https://github.com/Sanj-dot/Portfolio.git

# Add all files
git add .

# Commit your changes
git commit -m "Complete portfolio website with contact form and database integration"

# Push to GitHub
git push -u origin main
```

### Method 3: Download and Upload

1. **Download project from Replit:**
   - Use Replit's download feature to get all files
   - Extract the zip file locally

2. **Clone your GitHub repository:**
   ```bash
   git clone https://github.com/Sanj-dot/Portfolio.git
   cd Portfolio
   ```

3. **Copy files and push:**
   ```bash
   # Copy all files from downloaded project
   git add .
   git commit -m "Complete portfolio website"
   git push origin main
   ```

## What's Being Pushed

Your repository will include:

### ✅ Complete Application Files
- All React frontend components
- Express.js backend with API routes
- PostgreSQL database schema
- Tailwind CSS styling
- Framer Motion animations

### ✅ Configuration Files
- `package.json` with all dependencies
- `vite.config.ts` for build configuration
- `tailwind.config.ts` for styling
- `drizzle.config.ts` for database
- `tsconfig.json` for TypeScript

### ✅ Documentation
- `README.md` with comprehensive project info
- `replit.md` with architecture details
- This `GITHUB_SETUP.md` guide

### ❌ Excluded Files (.gitignore)
- `node_modules/` - Dependencies (will be installed via npm)
- `dist/` - Build output (generated during deployment)
- `.env` - Environment variables (you'll need to set these)
- `.replit` - Replit-specific files

## Post-Push Setup

After pushing to GitHub, you'll need to:

1. **Set up GitHub Pages** (optional):
   - Go to repository Settings > Pages
   - Select source branch (usually `main`)
   - Your site will be available at `https://sanj-dot.github.io/Portfolio`

2. **Configure Environment Variables** for deployment:
   - `DATABASE_URL` - Your PostgreSQL connection string
   - Any other secrets needed for production

3. **Update README** with your live URL once deployed

## Need Help?

If you encounter any issues:
1. Check that your GitHub repository exists at `https://github.com/Sanj-dot/Portfolio`
2. Ensure you have push permissions to the repository
3. Verify your Git configuration is correct
4. Try the Replit Git integration first as it's the simplest method

Your portfolio is complete and ready to be shared with the world! 🚀