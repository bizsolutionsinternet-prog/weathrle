# 🌍 WEATHRLE - Daily Weather Temperature Game

A daily weather guessing game where players predict high temperatures in 3 cities around the world.

## 📋 Files Overview

### Core Files
- `weathrle-final.html` - Main game file (upload as `index.html`)
- `robots.txt` - Search engine instructions
- `sitemap.xml` - Site structure for SEO
- `manifest.json` - PWA (installable app) configuration
- `.htaccess` - Server configuration (Apache only)

## 🖼️ Images You Need to Create

### 1. **Open Graph Image** (Social Media Sharing)
- **Filename:** `og-image.png`
- **Size:** 1200 x 630 pixels
- **Content:** Logo + screenshot + "Daily Weather Challenge" text
- **Used when:** Someone shares on Facebook, Twitter, WhatsApp, LinkedIn

### 2. **PWA Icons** (Mobile Install)
- **icon-192.png** - 192 x 192 pixels
- **icon-512.png** - 512 x 512 pixels
- **Content:** WEATHRLE logo with 🌍 emoji or weather theme
- **Used when:** Users install app on mobile home screen

### 3. **Screenshot** (PWA Store)
- **screenshot-1.png** - 540 x 720 pixels
- **Content:** Game screenshot showing the interface
- **Used in:** App stores and install prompts

## 🚀 Deployment Steps

### Option 1: Simple Hosting (Netlify, Vercel, GitHub Pages)
1. Rename `weathrle-final.html` to `index.html`
2. Upload all files to your hosting
3. Create the required images (see above)
4. Update `sitemap.xml` with current date
5. Done! ✅

### Option 2: Traditional Hosting (cPanel, FTP)
1. Upload all files to `public_html` or `www` folder
2. Rename `weathrle-final.html` to `index.html`
3. Ensure `.htaccess` is uploaded (Apache servers only)
4. Create images
5. Test HTTPS is working

## 🔧 Configuration

### Update Domain in Files
Replace `https://weathrle.com` with your actual domain in:
- `weathrle-final.html` (meta tags)
- `sitemap.xml`
- `manifest.json` (start_url)

### Update Sitemap Date
In `sitemap.xml`, change:
```xml
<lastmod>2025-02-11</lastmod>
```
To today's date when you deploy.

## 📊 Analytics (Optional)

Add Google Analytics by inserting before `</head>`:
```html
<!-- Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=G-XXXXXXXXXX"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'G-XXXXXXXXXX');
</script>
```

## 🔍 SEO Checklist

- [ ] Images created and uploaded
- [ ] Domain updated in all files
- [ ] `robots.txt` accessible at `yourdomain.com/robots.txt`
- [ ] `sitemap.xml` accessible at `yourdomain.com/sitemap.xml`
- [ ] Submit sitemap to Google Search Console
- [ ] Test Open Graph with [OpenGraph.xyz](https://www.opengraph.xyz/)
- [ ] Test mobile responsiveness
- [ ] Test PWA install on mobile

## 🎨 Design Tools for Images

### Free Tools:
- **Canva** - Easy templates for og-image and icons
- **Figma** - Professional design tool
- **Photopea** - Free Photoshop alternative online

### Quick Tips:
- Use the 🌍 emoji prominently in icons
- Keep text readable on mobile for og-image
- Use the color scheme: Orange (#f59e0b) and light gray (#f9fafb)

## 📱 PWA Features

Your game can be installed like an app! Users will see an "Install" button in their browser.

**To enable:**
1. Create the icon images (192px and 512px)
2. Upload `manifest.json`
3. Add to HTML (already included):
```html
<link rel="manifest" href="/manifest.json">
```

## 🌐 Browser Support

- ✅ Chrome/Edge (full support)
- ✅ Safari (full support)
- ✅ Firefox (full support)
- ✅ Mobile browsers (optimized)

## 🔐 Security Notes

The `.htaccess` file includes:
- Force HTTPS redirect
- Security headers (XSS protection, clickjacking prevention)
- File compression
- Browser caching

If using Nginx instead of Apache, you'll need different configuration.

## 📈 Monitoring

Recommended tools:
- **Google Search Console** - Track SEO performance
- **Google Analytics** - User behavior
- **Cloudflare** - CDN and DDoS protection (free tier available)

## 🆘 Troubleshooting

**Issue:** Images not showing
- Check file paths are correct
- Ensure images are uploaded to root directory

**Issue:** PWA not installable
- Check manifest.json is accessible
- Verify HTTPS is enabled
- Create icon-192.png and icon-512.png

**Issue:** Not ranking in Google
- Submit sitemap to Search Console
- Wait 1-2 weeks for indexing
- Share on social media for backlinks

## 📞 Support

Created by an environmental engineer and climate advocate.

For issues or suggestions, update the code or consult web development documentation.

---

**License:** Free to use and modify
**Version:** 1.0
**Last Updated:** February 2025
