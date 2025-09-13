# Deploy PromptGenie AI to Vercel

## Quick Deployment Steps

### Option 1: Deploy via Vercel CLI (Recommended)
1. Install Vercel CLI: `npm i -g vercel`
2. Login to Vercel: `vercel login`
3. Deploy: `vercel --prod`

### Option 2: Deploy via GitHub Integration
1. Push code to GitHub repository
2. Connect GitHub repo to Vercel dashboard
3. Vercel will auto-deploy on commits

### Option 3: Deploy via Vercel Dashboard
1. Visit [vercel.com](https://vercel.com)
2. Import your project
3. Vercel will detect Expo and deploy automatically

## Environment Variables (Required for PayPal)
Add these in Vercel dashboard under Settings > Environment Variables:
- `EXPO_PUBLIC_PAYPAL_CLIENT_ID` - Your PayPal Client ID from PayPal Developer Dashboard
- `NODE_ENV` - Set to 'production' for live payments, 'development' for sandbox

## PayPal Setup Instructions
1. Go to https://developer.paypal.com/
2. Create a PayPal Developer account
3. Create a new app in your dashboard
4. Copy the Client ID for your environment (Sandbox for testing, Live for production)
5. Add the Client ID to your environment variables
## Custom Domain
1. Go to Vercel project settings
2. Add your custom domain
3. Update DNS records as instructed

## Monetization Ready
Your app includes:
- Payment integration ready
- User authentication
- Subscription tiers
- Terms & Privacy Policy
- Professional UI/UX

Start earning immediately after deployment!