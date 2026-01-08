# GitHub Pages Deployment

This repository is configured to host the workshop slides on GitHub Pages.

## 📍 Slides URL

Once published, your slides will be available at:
```
https://yourusername.github.io/github-workshop/slides/
```

Replace `yourusername` with your actual GitHub username.

## 🚀 Setup Instructions

### Option 1: Enable GitHub Pages (Easiest)

1. Go to your repository on GitHub
2. Click **Settings** tab
3. Click **Pages** in the left sidebar
4. Under **Source**, select:
   - Branch: `main`
   - Folder: `/ (root)`
5. Click **Save**
6. Wait 1-2 minutes for deployment
7. Visit: `https://yourusername.github.io/github-workshop/slides/`

### Option 2: Using GitHub Actions (Advanced)

A GitHub Actions workflow can automatically deploy changes. This is already configured if you have `.github/workflows/pages.yml`.

## 🎨 Customizing the Slides

### Change Theme

Edit `slides/index.html` and replace the theme CSS:

```html
<!-- Current theme (night) -->
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/reveal.js@4.5.0/dist/theme/night.css">
```

Available themes:
- `black.css` - Black background
- `white.css` - White background
- `league.css` - Gray background with blue accents
- `beige.css` - Beige colors
- `sky.css` - Blue colors
- `night.css` - Dark theme (current)
- `serif.css` - Serif fonts
- `simple.css` - Minimal
- `solarized.css` - Solarized colors
- `moon.css` - Dark blue
- `blood.css` - Dark red

### Add Your Branding

Update the final slide with your repository URL:

```html
<p class="small">Workshop materials:<br>
<a href="https://github.com/yourusername/github-workshop">github.com/yourusername/github-workshop</a></p>
```

## ⌨️ Keyboard Controls

During presentation:

- **Space** or **→** - Next slide
- **←** - Previous slide
- **Esc** or **O** - Overview mode (see all slides)
- **F** - Fullscreen
- **S** - Speaker notes (if available)
- **B** or **.** - Pause (black screen)
- **?** - Help menu

## 📝 Adding Speaker Notes

Add speaker notes to any slide:

```html
<section>
    <h2>Slide Title</h2>
    <p>Slide content</p>
    
    <aside class="notes">
        These are speaker notes.
        Press 'S' during presentation to view them.
    </aside>
</section>
```

## 🎯 Tips for Presenting

1. **Test beforehand**: Open slides in the browser you'll use for presenting
2. **Use overview mode**: Press `Esc` to see all slides
3. **Practice navigation**: Get comfortable with keyboard controls
4. **Fullscreen**: Press `F` for distraction-free presenting
5. **Print backup**: File → Print → Save as PDF for offline backup

## 🔧 Local Development

To test slides locally:

1. **Simple option**: Open `slides/index.html` directly in your browser
2. **Local server** (recommended for testing):
   ```bash
   cd slides
   python -m http.server 8000
   # Or: python3 -m http.server 8000
   ```
   Then visit: `http://localhost:8000`

## 📱 Mobile/Touch Controls

- Swipe left/right to navigate
- Pinch to zoom
- Two-finger tap for overview

## 🌐 Sharing the Slides

Share the GitHub Pages URL with:
- Workshop participants (for reference during/after workshop)
- Other facilitators
- Anyone interested in the content

The slides work on any modern browser, no installation required!

## ❓ Troubleshooting

**Slides not showing up?**
- Wait 1-2 minutes after enabling GitHub Pages
- Check Settings → Pages for deployment status
- Ensure `slides/index.html` exists in your repository
- Try hard refresh: Ctrl+Shift+R (Windows) or Cmd+Shift+R (Mac)

**Slides look broken?**
- Check browser console for errors (F12)
- Ensure you have internet connection (CDN resources)
- Try a different browser

**Can't navigate slides?**
- Make sure JavaScript is enabled
- Try keyboard navigation instead of mouse
- Check for browser extensions that might interfere

---

**Enjoy your presentation! 🎉**
