# 🚀 Complete Vercel Deployment Guide for PromptGenie AI

## Quick Start (5 Minutes to Live!)

### 1. Prepare Your Code
```bash
# Make sure all changes are committed
git add .
git commit -m "Ready for deployment"
```

### 2. Deploy via Vercel Dashboard (Easiest)
1. **Go to [vercel.com](https://vercel.com)**
2. **Sign in with GitHub** (creates account if needed)
3. **Click "New Project"**
4. **Select your repository** (or import from GitHub)
5. **Configure project:**
   - Framework Preset: `Other`
   - Build Command: `npm run build`
   - Output Directory: `dist`
   - Install Command: `npm install`
6. **Click "Deploy"** ✨

### 3. Set Environment Variables
In Vercel dashboard → Settings → Environment Variables:

**Required:**
```
EXPO_PUBLIC_PAYPAL_CLIENT_ID=your_paypal_client_id_here
NODE_ENV=production
```

**Optional but Recommended:**
```
EXPO_PUBLIC_APP_NAME=PromptGenie AI
EXPO_PUBLIC_SUPPORT_EMAIL=support@yourapp.com
```

### 4. Get PayPal Client ID
1. Go to [developer.paypal.com](https://developer.paypal.com)
2. Login/Create PayPal Developer account
3. Click "Create App"
4. Choose "Default Application" 
5. Copy the **Client ID** (not secret!)
6. Add to Vercel environment variables

## Alternative: Vercel CLI Method

```bash
# Install Vercel CLI
npm i -g vercel

# Login to Vercel
vercel login

# Deploy (follow prompts)
vercel

# Deploy to production
vercel --prod
```

## Troubleshooting Common Issues

### ❌ Build Fails
```bash
# Check these in Vercel dashboard:
- Environment variables are set correctly
- Build command is: npm run build
- Output directory is: dist
- Node.js version is 18.x or higher
```

### ❌ Blank White Screen
- Check browser console for errors
- Verify all environment variables are set
- Try hard refresh (Ctrl+F5)

### ❌ PayPal Not Working
- Verify PayPal Client ID is correct
- Check it's for the right environment (sandbox vs live)
- Ensure domain is added to PayPal app settings

### ❌ "Module Not Found" Errors
```bash
# Clear cache and redeploy
vercel --prod --force
```

## Post-Deployment Checklist

✅ **Test Core Features:**
- [ ] App loads without errors
- [ ] Navigation works
- [ ] Prompt generation works
- [ ] PayPal payment flow works
- [ ] All pages/modals display correctly

✅ **Performance Check:**
- [ ] Page loads in under 3 seconds
- [ ] Images display properly
- [ ] Mobile responsive design works

✅ **SEO & Analytics:**
- [ ] Add custom domain (optional)
- [ ] Set up Google Analytics (optional)
- [ ] Test social media sharing

## Your App is Now Live! 🎉

**Next Steps:**
1. Share your live URL with users
2. Monitor performance in Vercel dashboard
3. Set up custom domain if desired
4. Start collecting payments via PayPal!

**Live URL Format:**
`https://your-project-name.vercel.app`

Need help? Check the Vercel documentation or reach out!