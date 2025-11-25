# ReceiptBox - iOS App Landing Page

A professional, responsive landing page for the ReceiptBox iOS app - Smart receipt management and expense tracking.

## 🚀 Quick Setup for GitHub Pages

### Step 1: Create GitHub Repository

1. Go to [GitHub](https://github.com) and sign in
2. Click the "+" icon in the top right and select "New repository"
3. Name your repository `ReceiptBox` (or `yourusername.github.io` for a user site)
4. Make sure it's set to **Public**
5. Don't initialize with README (we already have one)
6. Click "Create repository"

### Step 2: Upload Your Files

**Option A: Using Command Line (Recommended)**

```bash
# Navigate to the ReceiptBox directory
cd /path/to/ReceiptBox

# Initialize git repository
git init

# Add all files
git add .

# Commit files
git commit -m "Initial commit: ReceiptBox landing page"

# Add your GitHub repository as remote
git remote add origin https://github.com/yourusername/ReceiptBox.git

# Push to GitHub
git branch -M main
git push -u origin main
```

**Option B: Using GitHub Desktop**

1. Download and install [GitHub Desktop](https://desktop.github.com/)
2. Click "Add" → "Add Existing Repository"
3. Select your ReceiptBox folder
4. Click "Publish repository" and follow the prompts

**Option C: Upload via GitHub Web Interface**

1. Go to your repository on GitHub
2. Click "Add file" → "Upload files"
3. Drag and drop all files and folders from your ReceiptBox directory
4. Click "Commit changes"

### Step 3: Enable GitHub Pages

1. Go to your repository on GitHub
2. Click "Settings" (top right)
3. Scroll down to "Pages" in the left sidebar
4. Under "Source", select:
   - Branch: `main`
   - Folder: `/ (root)`
5. Click "Save"
6. Wait 1-2 minutes for your site to deploy

### Step 4: Access Your Site

Your site will be available at:
- **Project site**: `https://yourusername.github.io/ReceiptBox/`
- **User site**: `https://yourusername.github.io/` (if you named the repo `yourusername.github.io`)

## 📁 Project Structure

```
ReceiptBox/
├── index.html          # Main landing page
├── support.html        # Support and FAQ page
├── privacy.html        # Privacy policy (required for App Store)
├── css/
│   └── style.css       # All styling
├── js/
│   └── main.js         # JavaScript functionality
├── images/             # Place your images here
│   ├── app-icon.png
│   ├── screenshot1.png
│   ├── screenshot2.png
│   └── screenshot3.png
└── README.md           # This file
```

## 🎨 Customization Guide

### 1. Update Text Content

Edit the HTML files to replace placeholder text with your actual content:

- **App name**: Search for "ReceiptBox" and replace if needed
- **Taglines and descriptions**: Update in `index.html`
- **Features**: Modify the feature cards in the Features section
- **Contact email**: Replace `support@receiptbox.app` with your email

### 2. Add Your App Screenshots

Replace the placeholder screenshot sections with actual iPhone screenshots:

1. Take screenshots of your app (iPhone recommended)
2. Save them as `screenshot1.png`, `screenshot2.png`, etc.
3. Place them in the `images/` folder
4. Update the image paths in `index.html`:

```html
<img src="images/screenshot1.png" alt="Main Dashboard">
<img src="images/screenshot2.png" alt="Scan Receipt">
<img src="images/screenshot3.png" alt="Analytics">
```

### 3. Add Your App Icon

1. Export your app icon as PNG (512x512 or 1024x1024)
2. Save as `app-icon.png` in the `images/` folder
3. Replace the emoji icon in the navigation with:

```html
<img src="images/app-icon.png" alt="ReceiptBox" width="40">
```

### 4. Update App Store Link

When your app is published, replace the `#` in the download buttons with your actual App Store URL:

```html
<a href="https://apps.apple.com/app/your-app-id" class="btn btn-primary">
```

### 5. Customize Colors

Edit the CSS variables in `css/style.css`:

```css
:root {
    --primary-color: #6366f1;      /* Main brand color */
    --secondary-color: #8b5cf6;     /* Secondary color */
    --accent-color: #ec4899;        /* Accent color */
}
```

### 6. Update Privacy Policy

Edit `privacy.html` to:
- Update the "Last Updated" date
- Replace email addresses with your actual contact emails
- Add any specific data collection practices for your app

## 🔧 Advanced Customization

### Adding Google Analytics

Add this code before the closing `</head>` tag in all HTML files:

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

### Custom Domain

To use your own domain (e.g., receiptbox.com):

1. Buy a domain from a registrar (Namecheap, Google Domains, etc.)
2. In your GitHub repository settings → Pages
3. Enter your custom domain
4. In your domain registrar's DNS settings, add:
   - Type: CNAME
   - Name: www
   - Value: yourusername.github.io

### Adding More Pages

Create new HTML pages following the same structure:
1. Copy the header and footer from existing pages
2. Link the new CSS file
3. Add navigation links in all pages

## 📱 Testing

Before going live, test your site:

1. **Local Testing**: Open `index.html` in a browser
2. **Responsive Testing**: Use browser dev tools (F12) to test mobile views
3. **Link Testing**: Click all navigation links to ensure they work
4. **Form Testing**: Test any contact forms or email links

## ✅ Pre-Launch Checklist

- [ ] All placeholder text replaced with actual content
- [ ] Real app screenshots added
- [ ] App icon added to images folder
- [ ] Privacy policy updated with correct information
- [ ] Support email addresses updated
- [ ] App Store link added (when available)
- [ ] All navigation links work correctly
- [ ] Site looks good on mobile devices
- [ ] Tested on multiple browsers (Chrome, Safari, Firefox)

## 🆘 Troubleshooting

### Site not showing up
- Wait 5-10 minutes after enabling GitHub Pages
- Check repository Settings → Pages for any error messages
- Ensure repository is Public, not Private

### Images not loading
- Check that image paths are correct (case-sensitive)
- Ensure images are in the `images/` folder
- Verify files were uploaded to GitHub

### Styling issues
- Clear your browser cache (Ctrl+F5 or Cmd+Shift+R)
- Check browser console (F12) for any errors
- Ensure `style.css` is in the `css/` folder

## 📞 Support

For questions about this template:
- Check the code comments in each file
- Review GitHub Pages documentation: https://pages.github.com/

## 📄 License

This template is free to use for your iOS app landing page. Feel free to customize it as needed!

---

**Good luck with your ReceiptBox app launch! 🚀**
