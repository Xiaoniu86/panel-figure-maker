# Deploy to Vercel

This guide will help you deploy Panel Figure Maker to Vercel in just a few minutes.

## Prerequisites

- GitHub account (for hosting the repository)
- Vercel account (free at https://vercel.com)

## Option 1: Deploy Directly from GitHub (Recommended)

### Step 1: Push to GitHub

1. Create a new GitHub repository named `panel-figure-maker`
2. Clone this repository locally:
   ```bash
   git clone <your-repo-url>
   cd panel-figure-maker
   ```

3. Add your files:
   ```bash
   git add .
   git commit -m "Initial commit: Panel Figure Maker"
   git push origin main
   ```

### Step 2: Deploy on Vercel

1. Go to [Vercel](https://vercel.com) and sign in with your GitHub account
2. Click **"Add New Project"**
3. Import your `panel-figure-maker` repository
4. Click **"Deploy"**
5. Wait ~30 seconds for deployment to complete
6. Your site is now live! 🎉

**Your URL will be:** `https://panel-figure-maker.vercel.app` (or custom domain)

## Option 2: Deploy via Vercel CLI

### Step 1: Install Vercel CLI

```bash
npm install -g vercel
```

### Step 2: Deploy

```bash
cd panel-figure-maker
vercel
```

Follow the prompts:
- Link to GitHub? → `Yes`
- Which scope? → Select your GitHub account
- Found existing project? → `No`
- Project name? → `panel-figure-maker`
- Which directory? → `.` (current directory)

Your site is now deployed! 🚀

## Option 3: Manual Deploy (No GitHub)

1. Visit [Vercel](https://vercel.com)
2. Upload the entire `panel-figure-maker` folder
3. Vercel will automatically deploy it

## After Deployment

- Your app is live and accessible to anyone with the URL
- All data is stored locally in user's browser (no backend needed)
- Auto-save functionality works out of the box
- You can continue editing `index.html` and redeploy

## Redeploy After Changes

If you make changes locally:

```bash
git add .
git commit -m "Update: Your changes here"
git push origin main
```

Vercel will automatically redeploy your changes.

## Custom Domain (Optional)

1. Go to your project on Vercel
2. Click **Settings** → **Domains**
3. Add your custom domain (e.g., `panelfigure.com`)
4. Follow DNS configuration instructions

## Troubleshooting

**Q: App loads but figures won't upload?**
- Ensure you're using a modern browser (Chrome, Firefox, Safari, Edge)
- Check browser console for errors (F12)

**Q: Changes not showing after push?**
- Vercel may take 30 seconds to redeploy
- Try hard refresh: `Ctrl+Shift+R` (Windows/Linux) or `Cmd+Shift+R` (Mac)

**Q: White blank page?**
- Check Vercel deployment logs for errors
- Ensure `index.html` is in the root directory

**Q: Storage not persisting?**
- localStorage works in most browsers
- Check if private/incognito mode is enabled
- Try a different browser

## Support

- [Vercel Documentation](https://vercel.com/docs)
- [Vercel Support](https://vercel.com/support)
- Create an issue in the GitHub repository

---

**Deployed successfully?** Star ⭐ the repository to show support!
