# Dayo - Legal & Policy Website

A lightweight, responsive static website for hosting legal and policy documents for a mobile application.

## 📁 Project Structure

```
dayo-terms/
├── index.html                      # Home page
├── terms.html                      # Terms of Service
├── privacy.html                    # Privacy Policy
├── community-guidelines.html       # Community Guidelines
├── refund-policy.html             # Refund Policy
├── virtual-currency-policy.html   # Virtual Currency Policy
├── payment-policy.html            # Payment Policy
├── data-deletion.html             # Data Deletion & Account Removal
├── style.css                      # Shared stylesheet
├── script.js                      # Mobile navigation script
└── README.md                      # This file
```

## 🎨 Design Features

- **Minimal & Modern**: Clean design with no framework dependencies
- **Fully Responsive**: Mobile-first design, works on all devices
- **Fast Loading**: Lightweight HTML + CSS (no bloat)
- **Semantic HTML**: Proper HTML5 semantic structure
- **Accessible**: WCAG compliant navigation and typography
- **Dark Footer**: Professional footer with organized links
- **Sticky Navigation**: Header stays visible while scrolling

## 📱 Pages Included

1. **index.html** - Home page with policy overview and navigation
2. **terms.html** - Terms of Service document
3. **privacy.html** - Privacy Policy document
4. **community-guidelines.html** - Community Guidelines
5. **refund-policy.html** - Refund and returns policy
6. **virtual-currency-policy.html** - In-app currency policy
7. **payment-policy.html** - Payment and billing policy
8. **data-deletion.html** - User data deletion procedures

## 🚀 Deployment

### GitHub Pages (Recommended)

1. Create a GitHub repository
2. Push all files to the repo
3. Go to **Settings → Pages → Source**
4. Select branch `main` or `master`
5. Save and your site will be live at `https://username.github.io/repo-name`

### Other Static Hosting

- **Netlify**: Drag & drop folder, connect GitHub for auto-deploy
- **Vercel**: Import repository and deploy
- **Firebase Hosting**: `firebase deploy`
- **Surge**: `surge` CLI command
- **Traditional Server**: Simply upload files via FTP/SFTP

## 🛠️ Customization

### Change App Name

Replace `YourApp` with your app name in:

- All HTML files (search and replace)
- style.css (if needed)

### Update Email Addresses

Find and replace:

- `support@yourapp.com` → your support email
- `privacy@yourapp.com` → your privacy email
- `billing@yourapp.com` → your billing email
- `legal@yourapp.com` → your legal email

### Replace Placeholder Content

Look for `<div class="placeholder">` elements in each HTML file and replace with actual policy text.

### Change Colors

Edit CSS variables in `style.css`:

```css
/* Primary color */
color: #0066cc; /* Change to your brand color */

/* Hero gradient */
background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
```

### Add Favicon

Add this to the `<head>` section of each HTML file:

```html
<link rel="icon" type="image/x-icon" href="favicon.ico" />
```

## 📝 Content Guidelines

Each policy page includes:

- **Title** - Policy name
- **Last Updated** - Date of last revision
- **Placeholder Sections** - Ready for your content:
  - Introduction
  - Scope/Key Terms
  - Policy Details
  - Contact Information

Replace placeholder text boxes with your actual policy content.

## ♿ Accessibility Features

- Semantic HTML5 elements
- Proper heading hierarchy
- Color contrast meets WCAG standards
- Mobile-friendly touch targets
- Keyboard navigation support
- Screen reader optimized

## 📊 Browser Compatibility

- Chrome/Edge (latest)
- Firefox (latest)
- Safari (latest)
- Mobile browsers (iOS Safari, Chrome Mobile)
- IE 11+ (basic support)

## ⚡ Performance

- **No external dependencies** - Pure HTML/CSS/JS
- **Lightweight**: ~50KB total (uncompressed)
- **Fast loading**: Optimized CSS and minimal JavaScript
- **Static hosting**: CDN-friendly

## 🔧 File Sizes

- HTML files: ~8-12KB each
- CSS: ~12KB
- JavaScript: ~1KB
- **Total**: ~100KB (all files)

## 📋 Navigation Menu

The navigation appears on all pages and includes:

- Home
- Terms
- Privacy
- Community
- Refund
- Currency Policy
- Payment Policy
- Data Deletion

## 🔐 Security Considerations

- Uses relative URLs (works anywhere)
- No external resources required
- No cookies or tracking by default
- Can be deployed with HTTPS

## 📱 Mobile Optimization

- Responsive breakpoints at 768px and 480px
- Touch-friendly navigation toggle
- Readable font sizes on all devices
- Optimal line lengths for readability
- Proper spacing on mobile

## 📞 Support Contacts

Default contacts (customize these):

- General Support: support@yourapp.com
- Privacy/GDPR: privacy@yourapp.com
- Billing: billing@yourapp.com
- Legal: legal@yourapp.com
- Moderation: moderation@yourapp.com
- Refunds: refunds@yourapp.com

## 📄 License

This template is provided as-is for legal documentation. Customize content according to your jurisdiction and business requirements.

## 🎯 Next Steps

1. Replace `YourApp` with your actual app name
2. Update email addresses to your contact info
3. Replace placeholder content with actual policies
4. Customize colors to match your brand
5. Deploy to your hosting platform
6. Test on mobile devices
7. Monitor for broken links

---

**Ready to deploy!** No build process, no dependencies, no configuration needed. Just upload and go.

#

#
