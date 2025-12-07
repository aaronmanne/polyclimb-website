# PolyClimb.net Website

Professional website for Poly Climb and other mobile puzzle games.

## Overview

This website serves as the homepage for Poly Climb, EchoCube, and LumaTap games. It includes all necessary pages required for App Store submission and provides a comprehensive online presence.

## Pages Included

- **index.html** - Homepage with game showcase
- **privacy.html** - Privacy Policy (required for App Store)
- **terms.html** - Terms of Service (required for App Store)
- **support.html** - Support & FAQ page (required for App Store)
- **contact.html** - Contact page
- **styles.css** - Complete stylesheet with neon gaming aesthetic

## Features

- Responsive design (mobile, tablet, desktop)
- Neon gaming aesthetic matching Poly Climb's visual style
- Smooth animations and transitions
- App Store compliance (Privacy Policy, Terms, Support URLs)
- SEO optimized with proper meta tags
- Accessibility-friendly navigation
- Information for all three games: Poly Climb, EchoCube, LumaTap

## Deployment to Squarespace

Since you're using Squarespace for hosting, here's how to use these files:

### Option 1: Custom Code Blocks (Recommended)

1. Log in to your Squarespace account
2. Create a new blank page for each HTML file
3. Add a "Code" block to each page
4. Copy the content between `<main>` and `</main>` from each HTML file
5. Paste into the Code block
6. For the CSS:
   - Go to Design → Custom CSS
   - Copy the entire `styles.css` content
   - Paste into the Custom CSS editor

### Option 2: Export/Import

1. You may need to adjust the HTML to work with Squarespace's page builder
2. Squarespace doesn't directly import HTML files, so you'll need to:
   - Create pages in Squarespace
   - Use Code blocks to insert the HTML content
   - Add the CSS to the Custom CSS section

### Option 3: External Hosting + Redirect

If Squarespace customization is too limiting:
1. Host these files on GitHub Pages, Netlify, or Vercel (all free)
2. Point your polyclimb.net domain to that hosting
3. Or keep Squarespace for the main site and use these for App Store URLs

## Required URLs for App Store Connect

When submitting to the App Store, you'll need to provide these URLs:

- **Privacy Policy URL:** `https://polyclimb.net/privacy.html`
- **Terms of Service URL:** `https://polyclimb.net/terms.html`
- **Support URL:** `https://polyclimb.net/support.html`
- **Marketing URL:** `https://polyclimb.net` (optional)

## Important Notes

### Email Address
Throughout the website, I've used `support@polyclimb.net` as the contact email. You'll need to:
1. Set up this email address with your domain
2. Or replace all instances with your actual support email

To replace the email:
```bash
# Find all instances
grep -r "support@polyclimb.net" .

# Replace with your email (example)
sed -i '' 's/support@polyclimb.net/your-email@example.com/g' *.html
```

### App Store Links
The "Download on App Store" buttons currently link to `#` (placeholder). Update these once your app is live:

Find and replace in all HTML files:
- Look for `<a href="#" class="btn btn-primary app-store-btn">`
- Replace `#` with your actual App Store link

Example App Store URL format:
```
https://apps.apple.com/us/app/poly-climb/id[YOUR-APP-ID]
```

### Game Descriptions
The descriptions for EchoCube and LumaTap are generic placeholders. Update them once you have more details about these games.

## Customization

### Colors
All colors are defined as CSS variables in `styles.css`:
```css
--primary-color: #00f3ff;     /* Cyan neon */
--secondary-color: #ff006e;   /* Pink neon */
--accent-color: #ffd60a;      /* Yellow accent */
--bg-dark: #0a0e27;          /* Dark blue background */
--bg-darker: #050814;        /* Darker background */
```

Change these to customize the entire color scheme.

### Content
All content is in plain HTML, making it easy to edit:
- Update game descriptions in `index.html`
- Modify FAQ entries in `support.html`
- Adjust legal text in `privacy.html` and `terms.html`

## Browser Support

- Chrome/Edge (latest)
- Firefox (latest)
- Safari (latest)
- Mobile browsers (iOS Safari, Chrome Mobile)

## Testing Locally

1. Open any HTML file directly in your browser
2. Or use a local server:
   ```bash
   # Python 3
   python3 -m http.server 8000
   
   # Then visit http://localhost:8000
   ```

## File Structure

```
website/
├── index.html      # Homepage
├── privacy.html    # Privacy Policy
├── terms.html      # Terms of Service
├── support.html    # Support & FAQ
├── contact.html    # Contact page
├── styles.css      # All styles
└── README.md       # This file
```

## Next Steps

1. Set up `support@polyclimb.net` email
2. Upload files to Squarespace (or alternative hosting)
3. Test all pages on mobile and desktop
4. Get your App Store link and update the download buttons
5. Use the URLs in App Store Connect submission
6. Update EchoCube and LumaTap descriptions when ready

## Support

If you need to make changes:
- Edit HTML files directly for content changes
- Edit `styles.css` for visual changes
- All pages use the same stylesheet for consistency

## Legal Compliance

This website includes:
- ✅ Privacy Policy with AdMob disclosures
- ✅ Terms of Service with Apple requirements
- ✅ Support page with FAQs
- ✅ Contact information
- ✅ App Store compliance language

All required for App Store submission!

---

**Built for:** Poly Climb, EchoCube, LumaTap  
**Domain:** polyclimb.net  
**Last Updated:** December 7, 2025
