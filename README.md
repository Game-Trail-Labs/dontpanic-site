# Don't Panic Website

Landing page, privacy policy, terms of service, and support for the Don't Panic iOS app.

## Setup

### 1. Create a New GitHub Repository

```bash
cd dontpanic-site
git init
git add .
git commit -m "Initial commit - landing page, privacy, terms, support"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/dontpanic-site.git
git push -u origin main
```

### 2. Enable GitHub Pages

1. Go to your repository on GitHub
2. Click **Settings** → **Pages**
3. Under "Source," select **Deploy from a branch**
4. Select **main** branch and **/ (root)**
5. Click **Save**

Your site will be live at: `https://YOUR-USERNAME.github.io/dontpanic-site`

### 3. Add Custom Domain (Optional)

#### Configure GitHub
1. In Settings → Pages → Custom domain
2. Enter `dontpanicapp.com`
3. Check "Enforce HTTPS"

#### Configure DNS (at your registrar)
Add these DNS records:

**A Records** (for apex domain `dontpanicapp.com`):
```
185.199.108.153
185.199.109.153
185.199.110.153
185.199.111.153
```

**CNAME Record** (for `www.dontpanicapp.com`):
```
YOUR-USERNAME.github.io
```

DNS changes can take up to 48 hours to propagate.

## Files

- `index.html` - Main landing page
- `privacy.html` - Privacy Policy
- `terms.html` - Terms of Service
- `support.html` - Support center with FAQ
- `style.css` - All styling
- `CNAME` - Custom domain configuration

## To Do Before Launch

- [ ] Add app screenshot (`screenshot.png`)
- [ ] Add favicon (`favicon.png`)
- [ ] Update App Store link when app is live
- [ ] Update email addresses if different from defaults
- [ ] Review and customize legal documents
- [ ] Add Google Analytics (optional)

## Customization

### Update App Store Links
Search and replace `https://apps.apple.com/app/dont-panic` with your actual App Store URL once the app is published.

### Update Email Addresses
Default emails used:
- `support@dontpanicapp.com`
- `privacy@dontpanicapp.com`
- `legal@dontpanicapp.com`
- `feedback@dontpanicapp.com`
- `bugs@dontpanicapp.com`

You can use email forwarding to route all these to one inbox.

### Add Screenshot
Replace `screenshot.png` with an actual iPhone screenshot of your app (ideally from the panic button or home screen).

## Domain Recommendations

Good domains to check availability:
- dontpanicapp.com ✓
- dontpanic.app
- getdontpanic.com
- trydontpanic.com

Registrar recommendations:
- **Cloudflare** (~$9/year) - includes free CDN, SSL, email forwarding
- **Namecheap** (~$10/year) - budget friendly
- **Google Domains** (~$12/year) - simple UI
