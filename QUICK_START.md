# Quick Start Guide - 5 Minutes to Customize Your Portfolio

## Step 1: Open the File
1. Locate `index.html` in your `portfolio4` folder
2. Right-click → Open with → Your favorite text editor (VS Code, Notepad++, etc.)

## Step 2: Essential Changes (Required)

### Change Your Name (3 places)
Find and replace these lines:
- **Line 22:** Change `Mohit Solanki` in navbar
- **Line 205:** Change `Mohit Solanki` in hero title  
- **Line 330-337:** Change `Mohit Solanki` in footer

**Quick Find:** Press `Ctrl+H` (Find & Replace) → Search: `Mohit Solanki` → Replace: `Your Name`

### Add Your Photo
- **Line 295:** Replace image URL
```html
<!-- OLD -->
<img src="https://via.placeholder.com/300x300?text=John+Doe" alt="Mohit Solanki">

<!-- NEW -->
<img src="YOUR_IMAGE_URL_OR_PATH" alt="Your Name">
```

**Quick Image Options:**
```
https://via.placeholder.com/300x300?text=Your+Name
https://ui-avatars.com/api/?name=Your+Name&background=667eea&color=fff
OR upload your own: /images/profile.jpg
```

## Step 3: Update Content (Recommended)

### Bio Section (Lines 293-296)
Replace example text with your real bio

### Skills (Lines 304-325)
Update skill names and percentages to match your abilities

### Projects (Lines 331-361)
Replace 3 sample projects with your real projects

### Social Links (Lines 334-337)
Add your actual LinkedIn, GitHub, Twitter URLs

## Step 4: Test Locally (Optional but Recommended)

### Windows PowerShell:
```powershell
cd d:\portfolio4
python -m http.server 8000
```

Then open: `http://localhost:8000`

### Mac/Linux Terminal:
```bash
cd ~/portfolio4
python3 -m http.server 8000
```

## Step 5: Deploy (Free Options)

### GitHub Pages (Easiest)
1. Create GitHub account (free)
2. Create new repo: `yourusername.github.io`
3. Upload `index.html`
4. Visit: `https://yourusername.github.io`

### Netlify (Fastest)
1. Drag & drop `index.html` to https://netlify.com
2. Get live URL instantly
3. No account needed!

### Vercel
Similar to Netlify, very easy

## Advanced: Connect Contact Form

Your form currently shows a "thank you" message demo.

### Option 1: Formspree (Free, 50 submissions/month)
1. Visit https://formspree.io
2. Sign up and create a new form
3. Copy your form ID
4. Update line 320:
```html
<!-- Change FROM: -->
<form class="contact-form" id="contactForm">

<!-- Change TO: -->
<form class="contact-form" action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
```
5. Remove or comment out the JavaScript validation if not needed

### Option 2: EmailJS (Free tier available)
1. Visit https://www.emailjs.com
2. Follow their setup guide
3. Update JavaScript in the file to use EmailJS

## Color Customization

Edit lines 19-26 in the `<style>` section:

```css
:root {
    --accent: #667eea;           /* Primary color - change this! */
    --accent-dark: #764ba2;      /* Darker shade */
    --bg-dark: #0f0f23;          /* Dark background */
    --text-light: #e0e0e0;       /* Text color */
}
```

**Popular color schemes:**
- **Blue:** `#667eea` → `#764ba2`
- **Green:** `#00d084` → `#00a853`
- **Purple:** `#9d4edd` → `#5a189a`
- **Orange:** `#ff6b35` → `#f7931e`
- **Pink:** `#ff006e` → `#d62828`

## Testing Checklist

- [ ] Name is updated everywhere
- [ ] Photo displays correctly
- [ ] All links work (social, navigation)
- [ ] Theme toggle works (moon/sun icon)
- [ ] Mobile menu works (hamburger on small screens)
- [ ] Form validates and shows message
- [ ] Animations smooth on scroll
- [ ] Looks good on phone/tablet

## Common Issues & Fixes

**Images not showing?**
- Check URL is correct
- If using local images: upload to same folder as index.html
- Use relative path: `./images/photo.jpg`

**Theme not saving?**
- Clear browser cache
- Check if browser has localStorage enabled

**Slow to load?**
- Compress images (use tinypng.com)
- Use smaller image files
- Use a CDN for images

## You're Done! 🎉

Your portfolio is ready to share:
- Send link to friends/employers
- Add to LinkedIn profile
- Include in resume
- Share on social media

---

**Questions?** Check README.md for detailed guide
**Need help?** Google "how to [what you want to do]" + "HTML CSS"

Good luck! 🚀
