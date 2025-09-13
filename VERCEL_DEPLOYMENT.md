# Deploy PromptGenie AI to Vercel - Step by Step Guide

## Prerequisites
- GitHub account
- Vercel account (free tier available)
- PayPal Developer account for payments

## Step 1: Push Code to GitHub
```bash
git init
git add .
git commit -m "Initial commit - PromptGenie AI"
git branch -M main
git remote add origin https://github.com/yourusername/promptgenie-ai.git
git push -u origin main
```

## Step 2: Deploy to Vercel

### Option A: Vercel Dashboard (Recommended)
1. Go to [vercel.com](https://vercel.com) and sign in
2. Click "New Project"
3. Import your GitHub repository
4. Vercel will auto-detect Expo and configure build settings
5. Click "Deploy"

### Option B: Vercel CLI
```bash
npm i -g vercel
vercel login
vercel --prod
```

## Step 3: Configure Environment Variables
In Vercel dashboard, go to Settings > Environment Variables and add:

**Required:**
- `EXPO_PUBLIC_PAYPAL_CLIENT_ID` = Your PayPal Client ID
- `NODE_ENV` = `production`

**Optional:**
- `EXPO_PUBLIC_APP_NAME` = `PromptGenie AI`
- `EXPO_PUBLIC_SUPPORT_EMAIL` = `support@yourapp.com`

## Step 4: PayPal Setup
1. Visit [developer.paypal.com](https://developer.paypal.com)
2. Create/login to PayPal Developer account
3. Create new app in dashboard
4. Copy Client ID from your app
5. Add Client ID to Vercel environment variables

## Step 5: Custom Domain (Optional)
1. In Vercel project settings, go to "Domains"
2. Add your custom domain
3. Update DNS records as instructed by Vercel

## Build Configuration
The app is pre-configured with:
- `vercel.json` for deployment settings
- Web-optimized build process
- Static export for fast loading

## Troubleshooting
- **Build fails**: Check environment variables are set
- **PayPal not working**: Verify Client ID is correct
- **Blank page**: Check browser console for errors

## Post-Deployment
- Test all features on live site
- Verify PayPal payments work
- Monitor performance in Vercel dashboard

Your PromptGenie AI app is now live and ready to generate revenue!