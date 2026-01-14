# ULTRA-SIMPLE VERSION - This WILL Work!

## Deploy Instructions:

1. **Delete your current site in Netlify**
   - Go to your site in Netlify
   - Settings → scroll to bottom → Delete site

2. **Download and deploy this new ZIP**
   - Download referral-app-ULTRA-SIMPLE.zip
   - Go to https://app.netlify.com/
   - Drag the ZIP onto Netlify

3. **Add your API key**
   - Project configuration → Environment variables
   - Add: `ANTHROPIC_API_KEY` = your key
   - **CRITICAL**: Go to Deploys → Trigger deploy → Clear cache and deploy

4. **Visit your site**
   - Should work immediately!

## What's Different?
This version has the MOST EXPLICIT configuration possible:
- `publish = "."` in netlify.toml (tells Netlify files are at root)
- `_redirects` file (alternative routing method)
- Absolutely minimal structure

## Files:
```
referral-simple/
├── index.html           ← Your app
├── netlify.toml         ← Config
├── _redirects           ← Routing
└── netlify/
    └── functions/
        └── generate-letter.js
```
