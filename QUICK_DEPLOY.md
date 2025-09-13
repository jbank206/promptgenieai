# Quick Vercel Deployment Guide

## 1. Deploy to Vercel (2 minutes)

### Option A: GitHub (Recommended)
1. Push your code to GitHub
2. Go to [vercel.com](https://vercel.com)
3. Click "Import Project" → Connect your GitHub repo
4. Vercel auto-detects Expo and deploys

### Option B: Vercel CLI
```bash
npm i -g vercel
vercel --prod
```

## 2. Environment Variables
Add these in Vercel dashboard → Settings → Environment Variables:
- `EXPO_PUBLIC_PAYPAL_CLIENT_ID`: Your PayPal client ID
- `NODE_ENV`: production

## 3. Custom Domain (Optional)
- Vercel dashboard → Domains → Add your domain

## 4. Fix Applied
✅ Fixed JSON parsing error in PayPal component with try-catch block

Your app is now ready for deployment!