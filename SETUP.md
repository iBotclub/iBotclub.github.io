# 🚀 Quick Setup Guide - iBot Website

## For New Contributors

### 1. First Time Setup

```bash
# Clone the repository
git clone https://github.com/iBotclub/iBotclub.github.io.git
cd iBotclub.github.io

# Install Ruby dependencies
gem install bundler
bundle install --path vendor/bundle

# Start local server
bundle exec jekyll serve --port 8080

# Visit http://localhost:8080 in your browser
```

### 2. Making Changes

#### Update Team Members
1. Navigate to `_data/core_25_26.yml` or `_data/cordis_25_26.yml`
2. Add your details following the existing format
3. Add your photo to `assets/images/core_25_26/` or `assets/images/cordi_25_26/`

#### Add Events
1. Edit `_data/events.yml`
2. Add event image to `assets/images/event/`
3. Create event page if needed in `event/` folder

#### Write Blog Posts
1. Create new file: `_posts/YYYY-MM-DD-your-post-title.md`
2. Use the following template:

```markdown
---
layout: post
title: "Your Awesome Title"
author: "Your Name"
date: 2025-12-07
---

Your content here...
```

#### Add Achievements
1. Edit `_data/achievements.yml`
2. Follow the existing format

### 3. Testing Locally

```bash
# Start development server
bundle exec jekyll serve --port 8080

# Build for production (before committing)
bundle exec jekyll build
```

### 4. Commit & Push

```bash
git add .
git commit -m "Description of your changes"
git push origin main
```

---

## Common Tasks

### Change Colors
Edit `css/modern-base.css` and modify the CSS variables:
```css
:root {
  --primary-red: #ff1717;  /* Change this */
}
```

### Add New Page
1. Create `new-page.html` in root directory
2. Add front matter:
```yaml
---
title: New Page
layout: default
style: new-page
permalink: /new-page/
---
```
3. Create `css/new-page.css` for styling
4. Add link to navigation in `_includes/header.html`

### Optimize Images
```bash
# Resize images before adding
# Recommended: 800x800px for team photos
# Recommended: 1200x600px for event banners
```

---

## Troubleshooting

### Jekyll won't start
```bash
bundle clean --force
bundle install
```

### Changes not showing
```bash
# Clear Jekyll cache
bundle exec jekyll clean
bundle exec jekyll serve
```

### Port already in use
```bash
# Use different port
bundle exec jekyll serve --port 8081
```

---

## Design Guidelines

### Color Palette
- Primary: `#ff1717` (iBot Red)
- Dark BG: `#0a0e27`
- Card BG: `#151932`
- Text: `#ffffff` (primary), `#b8c5d6` (secondary)

### Typography
- Headings: Archivo Black (bold, uppercase for effect)
- Body: Poppins (clean, readable)
- Code: Courier New (monospace)

### Spacing
- Section padding: 4-6rem
- Card padding: 2rem
- Element gaps: 1-2rem

### Responsive Breakpoints
- Desktop: 1200px+
- Tablet: 768px - 1199px
- Mobile: < 768px

---

## File Naming Conventions

- **HTML**: lowercase-with-hyphens.html
- **CSS**: lowercase-with-hyphens.css
- **Images**: lowercase-with-hyphens.jpg/png
- **Blog Posts**: YYYY-MM-DD-title-with-hyphens.md
- **Data**: lowercase_with_underscores.yml

---

## Need Help?

- Check the [main README](README.md)
- Contact: ibot_cfi@smail.iitm.ac.in
- Join our meetings for guidance

---

**Happy Coding! 🤖**
