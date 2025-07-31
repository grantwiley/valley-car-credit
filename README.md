# Valley Car Credit Website

A fully responsive, accessible static website for Valley Car Credit, designed for deployment on Sevalla hosting.

## 🚀 Quick Start

This is a static website that can be deployed directly to any web hosting service. No build process or server-side dependencies required.

### Deployment to Sevalla

1. **Upload Files**: Copy all files and folders to your Sevalla hosting directory
2. **Update Base URL**: Replace `https://valleycarcredit.com` with your actual domain in all HTML files
3. **Configure Domain**: Point your domain to the hosting directory
4. **Test**: Verify all pages load correctly

### File Structure

```
valley-car-credit/
├── index.html                 # Homepage
├── online-account.html        # Account management page
├── make-payment.html          # Payment page
├── credit-improvement.html    # Credit improvement guide
├── resources.html             # External resources
├── contact.html               # Contact page
├── css/
│   └── styles.css            # Main stylesheet
├── js/
│   └── main.js               # JavaScript functionality
├── blog/
│   ├── index.html            # Blog listing page
│   └── understanding-your-credit-report.html # Sample blog post
├── images/                   # Image assets (create this directory)
├── docs/                     # Original documents
└── README.md                 # This file
```

## 🎨 Customization

### Colors and Branding

The site uses CSS custom properties for easy customization. Edit `css/styles.css`:

```css
:root {
    --primary-color: #1e3a8a;      /* Main brand color */
    --secondary-color: #059669;     /* Secondary color */
    --accent-color: #f59e0b;        /* Accent color */
    /* ... other variables */
}
```

### Logo

1. Replace `/images/vcc-logo.jpg` with your actual logo
2. Update logo dimensions in CSS if needed
3. Ensure logo has good contrast and is readable

### Contact Information

Update contact information in all HTML files:
- Phone: 540-213-0202
- Email: info@valleycarcredit.com
- Address: 537 Richmond Avenue, Staunton, VA 24401

### External Links

Update these links in the appropriate pages:
- Account portal: `https://www.myfexaccount.com`
- Payment portal: `https://mxmerchant.com/mxcustomer/d/d4fcac2c-9dcf-4a1a-a2e7-44ae8ae210f5/v3`

## 📝 Adding Blog Posts

### Method 1: HTML Files (Recommended)

1. Create a new HTML file in the `blog/` directory
2. Use the existing blog post template structure
3. Update the blog index page to include the new post
4. Add appropriate meta tags and SEO information

### Method 2: Markdown with Frontmatter

If you prefer Markdown, you can create `.md` files with frontmatter:

```markdown
---
title: "Your Blog Post Title"
date: "2024-01-20"
category: "Credit Tips"
tags: ["credit", "education", "tips"]
excerpt: "Brief description of the post"
---

Your blog post content here...
```

Then convert to HTML using a simple static site generator or manual conversion.

## 🔧 Configuration

### Site Metadata

Create a `_config.js` file for centralized site configuration:

```javascript
const siteConfig = {
    title: "Valley Car Credit",
    description: "Auto financing and credit rebuilding in Staunton, VA",
    url: "https://valleycarcredit.com",
    phone: "540-213-0202",
    email: "info@valleycarcredit.com",
    address: {
        street: "537 Richmond Avenue",
        city: "Staunton",
        state: "VA",
        zip: "24401"
    }
};
```

### SEO Optimization

Each page includes:
- Meta descriptions
- Open Graph tags
- Canonical URLs
- Structured data (JSON-LD)
- Semantic HTML

### Performance

The site is optimized for:
- Fast loading (minimal dependencies)
- Mobile-first responsive design
- Accessibility (WCAG 2.1 AA compliant)
- SEO best practices

## 🛠️ Features

### Accessibility

- Skip navigation links
- ARIA labels and roles
- Keyboard navigation support
- High contrast ratios
- Screen reader friendly

### Mobile Responsive

- Mobile-first design approach
- Hamburger menu for mobile
- Touch-friendly buttons
- Optimized typography

### Interactive Elements

- Mobile navigation toggle
- Accordion sections
- Form validation
- Smooth scrolling
- Loading states

## 📱 Chat Integration

### Current Setup

The site includes a placeholder chat widget. To integrate a real chat service:

### Option 1: Chekkit Integration

1. Sign up at [chekkit.com](https://chekkit.com)
2. Get your widget code
3. Replace the chat widget placeholder in all HTML files
4. Update the JavaScript to handle chat functionality

### Option 2: Other Chat Services

Replace the chat widget with your preferred service:
- LiveChat
- Intercom
- Zendesk Chat
- Custom solution

## 🗺️ Google Maps Integration

### Current Setup

The contact page includes a placeholder for Google Maps. To add the actual map:

1. Go to [Google Maps](https://maps.google.com)
2. Search for "537 Richmond Avenue, Staunton, VA"
3. Click "Share" and select "Embed a map"
4. Copy the iframe code
5. Replace the placeholder in `contact.html`

## 📊 Analytics

### Google Analytics

Add Google Analytics by including the tracking code in the `<head>` section of all HTML files:

```html
<!-- Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=GA_MEASUREMENT_ID"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'GA_MEASUREMENT_ID');
</script>
```

### Other Analytics

You can add any analytics service by including the appropriate tracking code.

## 🔒 Security

### HTTPS

Ensure your hosting provider supports HTTPS and redirects all HTTP traffic to HTTPS.

### Form Security

The contact form currently uses `mailto:` as a fallback. For better functionality:

### Option 1: Formspree

1. Sign up at [formspree.io](https://formspree.io)
2. Update the form action in `contact.html`
3. Test the form submission

### Option 2: Netlify Forms

If using Netlify hosting, add `netlify` attribute to forms for automatic handling.

## 📧 Email Configuration

### Contact Form

The contact form can be configured in several ways:

1. **Mailto (Current)**: Opens user's email client
2. **Formspree**: Free form handling service
3. **Custom Backend**: Server-side form processing
4. **Email Service**: Integration with services like SendGrid

## 🚀 Performance Optimization

### Images

- Optimize all images for web
- Use appropriate formats (JPEG for photos, PNG for graphics)
- Consider WebP format for better compression
- Implement lazy loading for blog images

### Caching

Configure your hosting provider to:
- Enable browser caching
- Compress static assets
- Use CDN for faster delivery

## 📱 Mobile Testing

Test the site on:
- iOS Safari
- Android Chrome
- Various screen sizes
- Different connection speeds

## 🔍 SEO Checklist

- [ ] All pages have unique titles and descriptions
- [ ] Open Graph tags are properly set
- [ ] Canonical URLs are correct
- [ ] Structured data is implemented
- [ ] Sitemap is generated (optional)
- [ ] robots.txt is configured (optional)

## 🛠️ Maintenance

### Regular Tasks

1. **Content Updates**: Keep blog posts and information current
2. **Link Checking**: Verify external links still work
3. **Performance Monitoring**: Check loading speeds
4. **Security Updates**: Keep dependencies updated
5. **Backup**: Regular backups of the site

### Adding New Pages

1. Create the HTML file
2. Update navigation menus
3. Add to sitemap (if using)
4. Test all links
5. Verify mobile responsiveness

## 📞 Support

For technical support or questions about the website:
- Email: info@valleycarcredit.com
- Phone: 540-213-0202

## 📄 License

This website is created for Valley Car Credit. All rights reserved.

---

**Last Updated**: January 2024
**Version**: 1.0.0 