# Rostr Landing Page

This is the landing page for getrostr.com.

## Setup Instructions

### 1. Add Screenshots
Save the following screenshot images to `docs/images/`:
- `screenshot-scheduler.png` - Scheduler view screenshot
- `screenshot-timeclock.png` - Time Clock view screenshot  
- `screenshot-staff.png` - Staff view screenshot
- `screenshot-reports.png` - Reports view screenshot

### 2. Add Favicon
Create a favicon from the logo and save as:
- `docs/images/favicon.png` (32x32 or 64x64)
- `docs/images/apple-touch-icon.png` (180x180)

### 3. Add OG Image
Create an Open Graph image (1200x630) for social sharing:
- `docs/images/og-image.png`

### 4. Update App Store Links
Edit `docs/index.html` and update the `APP_LINKS` object at the top of the JavaScript:

```javascript
const APP_LINKS = {
    playStore: 'https://play.google.com/store/apps/details?id=com.rostr.app',
    appStore: 'https://apps.apple.com/app/rostr/id000000000', // Update with iOS link
};
```

## Deployment

### Option 1: GitHub Pages
1. Push the `docs` folder to GitHub
2. Go to repo Settings → Pages
3. Set source to "Deploy from a branch" → `main` → `/docs`
4. Set custom domain to `getrostr.com`

### Option 2: Netlify / Vercel
1. Connect repo to Netlify/Vercel
2. Set build directory to `docs`
3. Configure custom domain `getrostr.com`

### Option 3: Manual Hosting
Upload contents of `docs` folder to your web host's public directory.

## DNS Configuration
Add these DNS records for your domain:
- For GitHub Pages: CNAME record pointing to `<username>.github.io`
- For Netlify: CNAME record as provided by Netlify
- For custom hosting: A record pointing to your server IP

## SEO Features Included
- ✅ Meta title & description
- ✅ Keywords meta tag
- ✅ Open Graph tags (Facebook, LinkedIn)
- ✅ Twitter Card tags
- ✅ Schema.org structured data (JSON-LD)
- ✅ Canonical URL
- ✅ Semantic HTML structure
- ✅ Mobile-responsive design
- ✅ Fast loading (no external JS frameworks)

## Files Structure
```
docs/
├── index.html          # Main landing page
├── privacy-policy.html # Privacy policy
├── terms-of-service.html # Terms of service
├── delete-account.html # Account deletion info
├── images/
│   ├── logo.png
│   ├── favicon.png
│   ├── apple-touch-icon.png
│   ├── og-image.png
│   ├── screenshot-scheduler.png
│   ├── screenshot-timeclock.png
│   ├── screenshot-staff.png
│   └── screenshot-reports.png
└── README.md
```
