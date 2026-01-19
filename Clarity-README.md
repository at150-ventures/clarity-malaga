# Mind Clarity Landing Page - Editing Guide

## 🎯 Quick Start

This HTML page is designed to be **super easy to edit** - even easier than Gamma! Everything you need to change is clearly marked with comments.

## 📝 How to Edit Content

### Common Changes (You'll do these most often)

**1. Change Text Content**
- Open `index.html` in any text editor (Notepad, TextEdit, VS Code, etc.)
- Search for the text you want to change
- Replace it with your new text
- Save the file

**2. Change Colors**
Look for this section at the top of the file (around line 25):
```css
:root {
    --primary-color: #2D5F7E;        /* Change this for main brand color */
    --accent-color: #E8956C;         /* Change this for button colors */
    --text-dark: #1A1A1A;
    --text-medium: #4A4A4A;
    --background-light: #F8F9FA;
}
```

**3. Change Prices**
Search for "€399" in the file and replace with your new price.

**4. Change Links**
Search for "https://tidycal.com/at150/mind-clarity-malaga" and replace with your booking link.

**5. Add/Remove FAQ Questions**
Find the FAQ section (search for "FAQ SECTION") and copy/paste this block:
```html
<div class="faq-item">
    <p class="faq-question">Your question here?</p>
    <p>Your answer here.</p>
</div>
```

## 🖼️ How to Add Images

Currently the page has placeholders that say "Replace with...". Here's how to add real images:

**Option 1: Upload images to the same folder**
1. Download images from Gamma
2. Put them in the same folder as `index.html`
3. Replace the placeholder sections with:
```html
<img src="your-image-name.jpg" alt="Description" style="width: 100%; border-radius: 12px;">
```

**Option 2: Use external image links**
1. Upload images to a service (Imgur, Cloudinary, your server)
2. Get the image URL
3. Replace placeholder with:
```html
<img src="https://your-image-url.com/image.jpg" alt="Description" style="width: 100%; border-radius: 12px;">
```

**Specific images to replace:**
- Brain scan visualization (around line 425)
- Profile photo of Robert-Jan (around line 575)
- Final CTA image (around line 610)

## 🚀 How to Publish

### Option 1: GitHub Pages (FREE & Easy)
1. Go to your GitHub account
2. Create a new repository called "mind-clarity" (or any name)
3. Upload `index.html` to the repository
4. Go to Settings → Pages
5. Select "main" branch, click Save
6. Your site will be live at: `https://yourusername.github.io/mind-clarity`

### Option 2: Netlify (FREE & Super Easy)
1. Go to netlify.com
2. Drag and drop your `index.html` file
3. Done! You get a URL instantly
4. You can connect your custom domain (clarity.at150.com)

### Option 3: Vercel (FREE & Fast)
1. Go to vercel.com
2. Sign up with GitHub
3. Import your repository
4. Done! Auto-deploys when you make changes

## 🔗 Connect Your Custom Domain

Once hosted, you'll need to update your DNS settings for clarity.at150.com:

**For GitHub Pages:**
- Add a CNAME record pointing to: `yourusername.github.io`

**For Netlify/Vercel:**
- They'll give you specific DNS instructions
- Usually an A record or CNAME

## 💡 Common Edits

### Add a New Testimonial
Copy this block (around line 515):
```html
<div class="testimonial">
    <p class="testimonial-text">"Your testimonial quote here"</p>
    <p class="testimonial-author">— Name, Title</p>
    <p class="testimonial-location">City, Country</p>
</div>
```

### Change Session Details
Find the "details-grid" section (around line 355) and edit the cards.

### Add New Benefits
Copy a "benefit-card" block and add your new benefit.

## 🎨 Design Tips

- **Keep it simple**: Don't change too much at once
- **Test on mobile**: Open the page on your phone to see how it looks
- **Use consistent colors**: Stick to the color variables defined at the top
- **Keep spacing consistent**: The design uses 2rem, 3rem spacing patterns

## 📱 Analytics Setup

To add Google Analytics:
1. Get your GA4 tracking code
2. Paste it just before `</head>` in the HTML (around line 15)

## 🐛 Troubleshooting

**Page looks broken after editing?**
- Check you didn't accidentally delete a `</div>` or `</section>` tag
- Make sure all quotation marks are closed properly

**Images not showing?**
- Check the file path is correct
- Make sure image files are in the same folder
- Check image file names match exactly (case-sensitive!)

**Colors not changing?**
- Make sure you're editing the CSS variables section
- Clear your browser cache (Cmd+Shift+R or Ctrl+F5)

## 💪 Advanced: Add Google Analytics

Want to track visitors? Here's how:

1. Get your Google Analytics tracking ID
2. Add this code just before `</head>`:

```html
<!-- Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=YOUR-GA-ID"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'YOUR-GA-ID');
</script>
```

## 🎓 Want to Learn More?

- HTML basics: https://www.w3schools.com/html/
- CSS basics: https://www.w3schools.com/css/
- Ask me (Claude) any questions!

## ✅ Checklist Before Publishing

- [ ] Replaced all placeholder images
- [ ] Updated booking link
- [ ] Added your profile photo
- [ ] Checked all text is correct
- [ ] Verified price is correct
- [ ] Tested on mobile (open on phone)
- [ ] Added analytics (optional)
- [ ] Tested all links work

---

**Need help?** Just ask! This page is designed to be simple enough for anyone to edit, but powerful enough to look professional.