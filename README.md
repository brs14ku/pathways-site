# Pathways Case Management Services - Website

A professional, fast-loading single-page website for Pathways Case Management Services.

## Features

- **Single-page design** with smooth scrolling navigation
- **Mobile-first responsive** design (optimized for all devices)
- **Fast loading** - No external dependencies, embedded CSS
- **Accessible** - WCAG AA compliant, semantic HTML, keyboard navigation
- **SEO optimized** - Meta tags, Open Graph tags, semantic structure
- **Email contact** - Contact and job-inquiry links open the visitor's email client (mailto), no form backend required

## Running Locally

There is no build step — the site is plain static files. Clone the repo and preview it:

```bash
git clone git@github.com:brs14ku/pathways-site.git
cd pathways-site
```

**Quick option:** Open `index.html` directly in your browser.

**Recommended:** Run a local static server so relative paths behave like production:

```bash
python3 -m http.server 8000
```

Then visit [http://localhost:8000](http://localhost:8000). (`python3` ships with macOS.) Node users can run `npx serve .` instead.

To make changes, edit `index.html` and refresh the browser.

## Deployment Options

### Option 1: GitHub Pages (Recommended)

1. Create a new repository on GitHub (e.g., `pathways-website`)
2. Push this code to the repository:
   ```bash
   git init
   git add .
   git commit -m "Initial commit"
   git branch -M main
   git remote add origin https://github.com/YOUR_USERNAME/pathways-website.git
   git push -u origin main
   ```
3. Go to repository Settings > Pages
4. Under "Source", select "main" branch
5. Save and wait a few minutes
6. Your site will be live at `https://YOUR_USERNAME.github.io/pathways-website/`

**Custom Domain Setup:**
1. In your repository, create a file named `CNAME` with your domain: `pathwayscms.com`
2. In your domain registrar's DNS settings, add:
   - A record pointing to: `185.199.108.153`
   - A record pointing to: `185.199.109.153`
   - A record pointing to: `185.199.110.153`
   - A record pointing to: `185.199.111.153`
3. Wait for DNS propagation (can take up to 24 hours)

### Option 2: Netlify

1. Create account at [netlify.com](https://www.netlify.com)
2. Drag and drop the `website` folder to Netlify dashboard
3. Your site will be live instantly with a Netlify URL

**Custom Domain on Netlify:**
1. Go to Site settings > Domain management
2. Add custom domain: `pathwayscms.com`
3. Follow Netlify's DNS configuration instructions
4. SSL certificate is automatically provisioned

## File Structure

```
website/
├── index.html          # Main website file (HTML + CSS + JS)
└── README.md          # This file
```

## Browser Support

- Chrome/Edge (last 2 versions)
- Firefox (last 2 versions)
- Safari (last 2 versions)
- Mobile browsers (iOS Safari, Chrome Mobile)

## Performance

- **Load time**: < 2 seconds
- **File size**: ~20KB HTML
- **No external dependencies**
- **Mobile-optimized images** (ready for WebP format)

## Customization

### Colors

Colors are defined in CSS variables at the top of the `<style>` section:

```css
:root {
    --primary-color: #2c7a7b;      /* Main teal color */
    --primary-dark: #234e52;       /* Darker teal */
    --accent-color: #d69e2e;       /* Gold accent */
    --text-dark: #2d3748;          /* Dark text */
    --text-light: #4a5568;         /* Light text */
}
```

### Content

All content is in `index.html`. Simply edit the text within the HTML tags.

## Maintenance

- **Regular updates**: Review and update content quarterly
- **Analytics**: Consider adding Google Analytics or Plausible for visitor tracking

## Support

For questions or issues with the website, contact: rschultz@pathwayscms.com

## License

Copyright 2026 Pathways Case Management Services. All rights reserved.
