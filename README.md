# Corvanta Partners - Website

🚀 Founder Growth & Execution Advisors

## About

Corvanta Partners helps founder-led companies scale from 20-200 people predictably. We provide strategic advisory, operational consulting, and fractional leadership support.

**Website:** https://corvantapartners.com  
**GitHub:** https://github.com/your-username/corvanta-website

---

## Website Structure

```
corvanta-website/
├── index.html              # Homepage
├── about.html              # About & Team
├── services.html           # Services Details
├── contact.html            # Contact Form
├── privacy-policy.html     # Privacy Policy
├── css/
│   └── style.css          # Shared stylesheet
├── js/
│   └── main.js            # JavaScript utilities
├── assets/
│   ├── favicon.png        # Favicon
│   └── founder-photo.jpeg # Founder photo
├── sitemap.xml            # SEO Sitemap
├── robots.txt             # Search engine robots
└── README.md              # This file
```

---

## Pages

### 1. **Homepage** (`index.html`)
- Hero section with founder problem statement
- Scaling journey visualization
- 3-problem identification cards
- 5-step operating system approach
- 3-tier service offerings
- Founder bio and stats
- Call-to-action section
- Navigation and footer

### 2. **About** (`about.html`)
- Mission statement
- Core beliefs
- Detailed founder biography
- Approach methodology
- Team stats and experience

### 3. **Services** (`services.html`)
- Growth Diagnostic details
- Transformation Sprint details
- Fractional Partner details
- Engagement journey visualization
- Service features and benefits

### 4. **Contact** (`contact.html`)
- Contact form (Formspree integration)
- Phone contact option
- Email contact option
- Post-contact process explanation
- Direct contact information

### 5. **Privacy Policy** (`privacy-policy.html`)
- Data collection practices
- Usage policies
- Security information
- Contact for privacy questions

---

## Design System

### Colors
- **Primary Dark:** #1A1A1A (Text, backgrounds)
- **Accent Orange:** #F2542D (Secondary highlights)
- **Accent Blue:** #1E6FD9 (Primary action)
- **Light Background:** #FBFAF7 (Section backgrounds)
- **Border:** #EEEEEE (Lines, dividers)
- **Gray:** #767676 (Secondary text)

### Typography
- **Headlines:** Sora (serif, 700)
- **Body:** DM Sans (sans-serif, 300-400)
- **Google Fonts imported from CDN**

### Components
- Navigation (sticky header)
- Hero sections
- Problem/solution cards
- Service tier cards
- Process step diagrams
- Contact forms
- Footer with links

---

## Installation & Setup

### Local Development

1. **Clone the repository:**
   ```bash
   git clone https://github.com/your-username/corvanta-website.git
   cd corvanta-website
   ```

2. **Open in browser:**
   - Simply open `index.html` in your browser
   - Or use a local server:
     ```bash
     python -m http.server 8000
     # Visit http://localhost:8000
     ```

### GitHub Pages Deployment

1. **Create GitHub repository:**
   - Go to github.com
   - Create new repository: `corvanta-website`
   - Make it public

2. **Upload files:**
   ```bash
   git add .
   git commit -m "Initial website deployment"
   git push origin main
   ```

3. **Enable Pages:**
   - Settings → Pages
   - Source: `main` branch (root)
   - Wait 1-2 minutes for deployment

4. **Access your site:**
   - `https://YOUR-USERNAME.github.io/corvanta-website`

### Custom Domain

1. **Update DNS:**
   - Point your domain to GitHub Pages
   - Add CNAME record: `USERNAME.github.io`

2. **GitHub Settings:**
   - Settings → Pages → Custom domain
   - Enter your domain (e.g., `corvantapartners.com`)
   - Enable HTTPS

---

## Customization

### Update Contact Information

Search and replace these across all files:

- **Email:** `pittlasanddeep@gmail.com` → Your email
- **Phone:** `+917337579994` → Your phone

### Update Founder Photo

1. Replace `assets/founder-photo.jpeg` with your photo
2. Update HTML to match:
   ```html
   <img src="assets/founder-photo.jpeg" alt="Your Name">
   ```

### Update Colors

Edit `css/style.css`:

```css
:root {
  --ink: #1A1A1A;
  --orange: #F2542D;
  --blue: #1E6FD9;
  --paper: #FBFAF7;
  --line: #EEEEEE;
  --grey: #767676;
}
```

### Update Fonts

In `index.html` and other pages, change Google Fonts import:

```html
<link href="https://fonts.googleapis.com/css2?family=YOUR-FONTS&display=swap" rel="stylesheet">
```

---

## SEO Optimization

### Meta Tags
- Title tags on every page
- Meta descriptions (155-160 chars)
- Open Graph tags (social sharing)
- Twitter Card tags
- Canonical URLs

### Technical SEO
- `robots.txt` for crawler guidance
- `sitemap.xml` for all pages
- Mobile responsive design
- Fast loading (CSS inline, optimized images)
- Semantic HTML structure

### To Improve Further
- Add blog section with keyword-optimized content
- Implement structured data (schema.org)
- Add Google Analytics tracking
- Submit sitemap to Google Search Console

---

## Form Integration

The contact form uses **Formspree** for email handling.

### How it Works

1. Form submits to Formspree endpoint
2. Formspree sends emails to your account
3. You receive inquiry emails directly

### Setup Formspree

1. Go to [formspree.io](https://formspree.io)
2. Sign up and create new form
3. Update form action in `contact.html`:
   ```html
   <form action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
   ```

### Alternative: EmailJS

If you prefer EmailJS:

```javascript
emailjs.init('YOUR_PUBLIC_KEY');

form.addEventListener('submit', function(e) {
  e.preventDefault();
  emailjs.sendForm('SERVICE_ID', 'TEMPLATE_ID', this);
});
```

---

## Analytics

### Google Analytics

Add to all pages before `</head>`:

```html
<script async src="https://www.googletagmanager.com/gtag/js?id=GA_ID"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'GA_ID');
</script>
```

Replace `GA_ID` with your Google Analytics 4 Property ID.

---

## Performance

- **CSS:** Embedded in HTML (single file)
- **JavaScript:** Minimal (smooth scroll, form handling)
- **Images:** Optimized JPEG/PNG
- **Fonts:** Google Fonts CDN
- **Mobile:** Responsive CSS with mobile-first approach

---

## Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Mobile browsers (iOS Safari, Chrome Mobile)

---

## Accessibility

- Semantic HTML (`<nav>`, `<section>`, `<footer>`)
- ARIA labels on form inputs
- Color contrast meets WCAG AA
- Keyboard navigation support
- Mobile responsive design

---

## Maintenance

### Regular Updates

**Monthly:**
- Check all links (internal and external)
- Test contact form
- Review analytics

**Quarterly:**
- Update team information
- Refresh testimonials/case studies
- Review and update copy

**Annually:**
- Security audit
- Performance optimization
- Content refresh

---

## Troubleshooting

### 404 Errors on GitHub Pages
- Check file paths (case-sensitive)
- Verify all files committed
- Clear browser cache

### Forms Not Working
- Verify Formspree integration
- Test with valid email
- Check spam folder

### Images Not Loading
- Verify file paths in HTML
- Ensure images in `assets/` folder
- Check image file names (case-sensitive)

### Styles Not Applied
- Clear browser cache (Ctrl+Shift+Delete)
- Check CSS file path
- Verify CSS file committed

---

## Support & Contact

**Website:** https://corvantapartners.com  
**Email:** pittlasanddeep@gmail.com  
**Phone:** +91 7337579994  
**LinkedIn:** linkedin.com/in/sanddeep

---

## License

© 2026 Corvanta Partners. All rights reserved.

---

## Changelog

### v1.0 (July 7, 2026)
- Initial website launch
- Homepage with hero, problem, approach, services
- About page with founder bio
- Services detail page
- Contact form integration
- Privacy policy
- SEO optimization
- Mobile responsive design
- GitHub Pages ready

---

**Ready to deploy? Push to GitHub and enable Pages!**
