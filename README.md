# KR Meditech Website

A professional medical equipment distributor website built with modern web technologies. This website showcases KR Meditech's diagnostic equipment distribution business with a clean, corporate design optimized for healthcare professionals.

## 🏥 Business Overview

**KR Meditech** is a leading distributor of medical and laboratory diagnostic equipment, serving hospitals, clinics, diagnostic centers, and laboratories. The website features:

- Product categories for diagnostic imaging, clinical lab analyzers, point-of-care devices, and pathology instruments
- Featured products showcase
- Brand partnerships display
- Comprehensive service offerings
- Professional contact and inquiry forms

## 🚀 Features

- **Responsive Design**: Optimized for desktop, tablet, and mobile devices
- **Modern UI/UX**: Clean, professional healthcare-themed design
- **Interactive Elements**: Smooth animations, hover effects, and transitions
- **Mobile Navigation**: Hamburger menu for mobile devices
- **Contact Form**: Functional contact form with validation
- **SEO Optimized**: Semantic HTML5 structure with proper meta tags
- **Performance Optimized**: Lazy loading and efficient CSS/JS
- **Accessibility**: Keyboard navigation and ARIA support

## 📁 Project Structure

```
KRMEDITECH/
├── index.html          # Main HTML file
├── styles.css          # Complete CSS styling
├── script.js           # JavaScript functionality
└── README.md          # This documentation
```

## 🛠️ Technologies Used

- **HTML5**: Semantic markup structure
- **CSS3**: Modern CSS with variables, Grid, and Flexbox
- **JavaScript (ES6+)**: Interactive features and form handling
- **Google Fonts**: Inter font family for professional typography
- **SVG Icons**: Custom SVG icons for scalability

## 🎨 Design System

### Color Palette
- **Primary**: `#0ea5e9` (Professional Blue)
- **Secondary**: `#16a34a` (Medical Green)
- **Accent**: `#f59e0b` (Warm Orange)
- **Neutral**: Various shades of gray for text and backgrounds

### Typography
- **Font Family**: Inter (Google Fonts)
- **Headings**: Bold weights (600-700)
- **Body Text**: Regular weight (400)
- **Responsive scaling** for all screen sizes

## 📱 Customization Guide

### 1. Updating Business Information

**Company Name & Logo:**
```html
<!-- In index.html, find the logo section -->
<h1 class="logo-text">KR<span class="logo-accent">Meditech</span></h1>
```

**Contact Information:**
```html
<!-- In the contact section -->
<div class="contact-text">
    <strong>Address:</strong><br>
    123 Medical Equipment Complex<br>
    Healthcare District, City - 123456
</div>
```

### 2. Replacing Placeholder Images

**Hero Section Image:**
```html
<!-- Replace the SVG placeholder with your image -->
<div class="hero-image">
    <img src="path/to/your/hero-image.jpg" alt="Medical Equipment">
</div>
```

**Product Images:**
```html
<!-- In product cards -->
<div class="product-image">
    <img src="path/to/product-image.jpg" alt="Product Name">
</div>
```

**Brand Logos:**
```html
<!-- In brands section -->
<div class="brand-logo">
    <img src="path/to/brand-logo.png" alt="Brand Name">
</div>
```

### 3. Updating Product Information

**Featured Products:**
```html
<div class="product-card">
    <div class="product-image">
        <!-- Product image -->
    </div>
    <div class="product-content">
        <h3 class="product-title">Your Product Name</h3>
        <p class="product-specs">• Spec 1<br>• Spec 2<br>• Spec 3</p>
        <button class="btn btn-outline">Learn More</button>
    </div>
</div>
```

### 4. Modifying Colors

**In styles.css, update CSS variables:**
```css
:root {
    --primary-color: #your-color;
    --secondary-color: #your-color;
    --accent-color: #your-color;
    /* ... other variables */
}
```

### 5. Adding New Sections

**To add a new section:**
1. Add HTML in `index.html` before the closing `</main>` tag
2. Add corresponding styles in `styles.css`
3. Add any JavaScript functionality in `script.js`

## 🚀 Deployment Instructions

### GitHub Pages Deployment

1. **Push to GitHub:**
   ```bash
   git init
   git add .
   git commit -m "Initial commit"
   git branch -M main
   git remote add origin https://github.com/yourusername/krmeditech.git
   git push -u origin main
   ```

2. **Enable GitHub Pages:**
   - Go to repository settings
   - Scroll to "Pages" section
   - Source: Deploy from a branch
   - Branch: main
   - Folder: /root
   - Save

3. **Access your site:**
   ```
   https://yourusername.github.io/krmeditech
   ```

### Vercel Deployment

1. **Install Vercel CLI:**
   ```bash
   npm i -g vercel
   ```

2. **Deploy:**
   ```bash
   vercel --prod
   ```

3. **Custom Domain:**
   - Add custom domain in Vercel dashboard
   - Update DNS records as instructed

### Netlify Deployment

1. **Drag and Drop:**
   - Drag the project folder to netlify.com
   - Or connect your GitHub repository

2. **Custom Domain:**
   - Add domain in Netlify dashboard
   - Update DNS records

## 🔧 Configuration

### Contact Form Setup

The contact form currently simulates submission. To make it functional:

1. **Replace with a form service:**
   ```html
   <form action="https://formspree.io/f/your-form-id" method="POST">
   ```

2. **Or integrate with a backend:**
   ```javascript
   // In script.js, update the form submission
   fetch('/api/contact', {
       method: 'POST',
       headers: { 'Content-Type': 'application/json' },
       body: JSON.stringify(data)
   })
   ```

### Analytics Integration

**Google Analytics:**
```html
<!-- Add to head section -->
<script async src="https://www.googletagmanager.com/gtag/js?id=GA_MEASUREMENT_ID"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'GA_MEASUREMENT_ID');
</script>
```

## 🌐 SEO Optimization

The website includes basic SEO optimization:

- **Meta Tags**: Title, description, and keywords
- **Semantic HTML**: Proper use of header, nav, main, section tags
- **Alt Text**: Image placeholders ready for alt attributes
- **Structured Data**: Ready for schema.org implementation

**To enhance SEO:**
1. Add specific meta descriptions for each section
2. Implement schema.org markup
3. Create an XML sitemap
4. Set up Google Search Console

## 📈 Performance Optimization

### Built-in Optimizations:
- **CSS Variables**: Efficient theming
- **Lazy Loading**: Images load when needed
- **Debounced Events**: Optimized scroll handlers
- **Minified Assets**: Ready for production

### Additional Optimizations:
1. **Image Optimization:**
   ```bash
   # Use tools like ImageOptim or Squoosh
   # Convert to WebP format for better compression
   ```

2. **Enable Gzip Compression:**
   - Configure server settings
   - Use build tools for compression

## 🐛 Troubleshooting

### Common Issues:

1. **Mobile Menu Not Working:**
   - Check if `script.js` is properly linked
   - Verify browser console for JavaScript errors

2. **Styles Not Loading:**
   - Ensure `styles.css` path is correct
   - Check file permissions

3. **Contact Form Issues:**
   - Verify form validation logic
   - Check browser console for errors

### Browser Support:
- **Modern Browsers**: Full support
- **IE 11**: Basic functionality (no grid/flexbox)
- **Mobile**: Full support on iOS Safari and Android Chrome

## 📞 Support

For technical support or customization requests:

1. **Check this README** for common solutions
2. **Review browser console** for JavaScript errors
3. **Validate HTML/CSS** using online validators
4. **Test on multiple devices** for responsive issues

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

---

**KR Meditech** © 2024 - Professional Medical Equipment Distribution
