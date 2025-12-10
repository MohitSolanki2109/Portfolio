# Mohit Solanki - Frontend Developer Portfolio

A modern, fully-responsive portfolio website with smooth animations, dark/light theme toggle, and mobile-optimized design. Built with **only HTML and CSS** (plus minimal vanilla JavaScript) - no external dependencies!

## ✨ Features

✅ **Responsive Design** - Perfect on desktop, tablet, and mobile
✅ **Dark/Light Theme** - Toggle between dark and light modes (saved in localStorage)
✅ **Smooth Animations** - Fade-ins, slide effects, hover animations, and floating shapes
✅ **Fast Loading** - No heavy libraries (Bootstrap, jQuery, etc.)
✅ **Accessibility** - Semantic HTML, proper ARIA labels, reduced motion support
✅ **SEO Optimized** - Proper meta tags, structured markup
✅ **Mobile Menu** - Hamburger menu for mobile devices
✅ **Active Navigation** - Auto-highlight current section in navbar
✅ **Contact Form** - Working form with validation and success messages
✅ **Cross-browser Compatible** - Works on all modern browsers

## 📁 File Structure

```
portfolio4/
├── index.html          # Complete website (HTML + embedded CSS + JavaScript)
├── index.css           # Standalone CSS (optional - for reference)
└── README.md           # This file
```

## 🚀 How to Use

### Option 1: Direct File Access
Simply open `index.html` in your web browser:
```
Double-click index.html
```

### Option 2: Local Server (Recommended for Testing)
```bash
# Using Python 3
python -m http.server 8000

# Using Python 2
python -m SimpleHTTPServer 8000

# Using Node.js (if installed)
npx http-server

# Using Node.js with npm
npm install -g http-server
http-server
```

Then visit: **http://localhost:8000/index.html**

## 🎨 Customization Guide

### 1. Change Your Name
Find and replace `"Mohit Solanki"` with your name in:
- Line 22: `<a href="#hero" class="navbar-brand">Mohit Solanki</a>`
- Line 205: `<h1>Hi, I'm <span>Mohit Solanki</span></h1>`
- Line 295: `<img src="..." alt="Mohit Solanki">`
- Line 330: `<p>&copy; 2024 Mohit Solanki. All rights reserved.</p>`
- Line 337: `<p>Designed & Built with ❤️ by Mohit Solanki</p>`

### 2. Update Your Photo
Replace the placeholder image URL at line 295:
```html
<img src="YOUR_IMAGE_URL_HERE" alt="Your Name">
```

**Get a free placeholder:**
- https://via.placeholder.com/300x300?text=Your+Name
- https://ui-avatars.com/api/?name=Your+Name&background=667eea&color=fff
- Upload your own image and use the path

### 3. Add Social Links
Update social links in footer (lines 334-337):
```html
<a href="https://linkedin.com/in/yourprofile" aria-label="LinkedIn">in</a>
<a href="https://github.com/yourprofile" aria-label="GitHub">gh</a>
<a href="https://twitter.com/yourprofile" aria-label="Twitter">tw</a>
```

### 4. Update Your Bio
Modify the about section text (lines 293-296):
```html
<p>I'm a frontend developer with 3+ years of experience...</p>
<p>When I'm not coding...</p>
```

### 5. Customize Skills
Update the skills section (lines 304-325) to match your proficiencies:
```html
<div class="skill-card">
    <h3>Your Skill</h3>
    <div class="progress-bar">
        <div class="progress-fill" style="--progress-width: 90%"></div>
    </div>
    <span class="skill-percent">90%</span>
</div>
```

### 6. Update Projects
Modify projects section (lines 331-361):
```html
<div class="project-card">
    <div class="project-image">🎨</div>
    <div class="project-content">
        <h3>Your Project Title</h3>
        <p>Your project description...</p>
        <div class="project-tags">
            <span class="project-tag">Technology 1</span>
            <span class="project-tag">Technology 2</span>
        </div>
    </div>
</div>
```

### 7. Setup Contact Form
The contact form currently shows a demo message. To make it work:

**Option A: Use Formspree (Free)**
1. Go to https://formspree.io
2. Sign up and create a form
3. Replace `id="contactForm"` with Formspree's form ID:
```html
<form class="contact-form" action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
```

**Option B: Use Email Service**
1. Use services like EmailJS, Netlify Forms, or AWS SES
2. Update the JavaScript handler accordingly

**Option C: Backend Integration**
1. Create a backend endpoint to handle form submissions
2. Update the JavaScript `fetch()` call to point to your endpoint

### 8. Change Colors (Optional)
Modify CSS variables at the top of the `<style>` tag (lines 19-26):
```css
:root {
    --accent: #667eea;              /* Primary color */
    --accent-dark: #764ba2;         /* Darker accent */
    --bg-dark: #0f0f23;             /* Dark background */
    --bg-light: #1a1a2e;            /* Slightly lighter bg */
    --text-light: #e0e0e0;          /* Text color */
    --text-muted: rgba(224, 224, 224, 0.6);
    --glass: rgba(255, 255, 255, 0.05);
    --glass-border: rgba(255, 255, 255, 0.1);
}
```

### 9. Deploy to the Web
Choose any of these free options:

**GitHub Pages:**
1. Create a repo named `username.github.io`
2. Push your files
3. Visit `https://username.github.io`

**Netlify:**
1. Drag & drop your `index.html` folder
2. Get a live URL instantly
3. (Optional) Connect a custom domain

**Vercel:**
1. Sign up at vercel.com
2. Import your GitHub repo
3. Auto-deploys on push

**Firebase Hosting:**
```bash
npm install -g firebase-tools
firebase login
firebase init hosting
firebase deploy
```

## 🔧 Browser Support

- ✅ Chrome/Edge (latest)
- ✅ Firefox (latest)
- ✅ Safari (latest)
- ✅ Mobile browsers (iOS Safari, Chrome Android)
- ✅ IE 11 (basic support, no CSS variables)

## 📱 Responsive Breakpoints

- **Desktop:** 1024px+
- **Tablet:** 768px - 1023px
- **Mobile:** 480px - 767px
- **Extra Small:** < 480px

## 🎭 Features Explained

### Dark/Light Theme Toggle
- Click the moon (🌙) / sun (☀️) icon in the navbar
- Theme preference is saved to browser localStorage
- Automatically loads on next visit

### Mobile Menu
- On mobile devices, menu collapses into a hamburger (☰)
- Click to toggle menu visibility
- Auto-closes when a link is clicked

### Active Navigation
- Current section is highlighted in navbar
- Updates automatically as you scroll
- Works on smooth scroll navigation

### Form Validation
- All fields are required
- Email format is validated
- Success/error messages display
- Form resets after submission

## ⚡ Performance Tips

1. **Optimize images** - Use WebP format or compress PNG/JPG
2. **Lazy loading** - Images load only when visible
3. **Caching** - Browser caches CSS and JS
4. **Minification** - Remove comments for production

## 🐛 Troubleshooting

**Theme not saving?**
- Check browser localStorage is enabled
- Clear browser cookies and try again

**Images not loading?**
- Verify image URLs are correct
- Check CORS if using external images
- Use absolute URLs for external sources

**Form not submitting?**
- Forms show demo messages by default
- Connect to a backend service (see Setup Contact Form)

**Animations not smooth?**
- Disable in accessibility settings if preferred
- Check GPU acceleration in browser settings

## 📈 SEO Optimization

The site includes:
- Meta descriptions
- Open Graph tags
- Semantic HTML
- Mobile viewport settings
- Fast loading times

To improve further:
1. Add Google Analytics
2. Create sitemap.xml
3. Add robots.txt
4. Use Google Search Console
5. Optimize images further

## 💡 Enhancement Ideas

- Add blog section
- Add testimonials carousel
- Add case studies
- Add downloadable CV
- Add work experience timeline
- Add email newsletter signup
- Add search functionality
- Add image gallery/portfolio grid

## 📝 License

Free to use and modify for personal and commercial projects.

## 🤝 Support

If you have questions or need help:
1. Check the comments in the code
2. Refer to this README
3. Search online for specific features
4. Consult MDN Web Docs

---

**Built with ❤️ using pure HTML, CSS, and JavaScript**

Happy coding! 🚀
