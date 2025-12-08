# 🎨 Quick Customization Guide

## Common Customizations for iBot Website

---

## 🎨 Change Colors

### Primary Color (Red)
**File**: `css/modern-base.css`

```css
:root {
  --primary-red: #ff1717;        /* Change to your color */
  --primary-red-dark: #cc0000;   /* Darker shade */
  --primary-red-light: #ff4444;  /* Lighter shade */
}
```

### Background Colors
```css
:root {
  --bg-dark: #0a0e27;      /* Main background */
  --bg-darker: #070b1f;    /* Darker areas */
  --bg-card: #151932;      /* Cards */
}
```

---

## 📝 Change Fonts

### Headings
**File**: `css/modern-base.css`

```css
:root {
  --font-display: 'Archivo Black', Arial, sans-serif;
}
```

**Update in**: `_includes/head.html`
```html
<link href="https://fonts.googleapis.com/css2?family=Your+Font&display=swap" rel="stylesheet">
```

### Body Text
```css
:root {
  --font-body: 'Poppins', Arial, sans-serif;
}
```

---

## 🖼️ Update Logo

1. Replace `assets/images/logo.png` with your logo
2. Recommended size: 200x200px PNG with transparency
3. Clear browser cache to see changes

---

## 👤 Add Team Member

**File**: `_data/core_25_26.yml` or `_data/cordis_25_26.yml`

```yaml
- name: "Your Name"
  image: "your-photo.jpg"
  mob: "+91 XXXXXXXXXX"
  email: "your.email@smail.iitm.ac.in"
  instagram: "https://instagram.com/username"
  linkedin: "https://linkedin.com/in/username"
  github: "https://github.com/username"
```

**Add photo**: `assets/images/core_25_26/your-photo.jpg`
- Size: 800x800px recommended
- Format: JPG or PNG

---

## 📅 Add Event

**File**: `_data/events.yml`

```yaml
- title: "Workshop: Introduction to ROS"
  date: "December 15, 2025"
  description: "Learn Robot Operating System basics"
  image: "/assets/images/event/ros-workshop.jpg"
  link: "/event/ros-workshop.html"
  button_text: "Register Now"
  disabled: false
  show_button: true
```

**Add image**: `assets/images/event/ros-workshop.jpg`
- Size: 1200x600px recommended

---

## 🤖 Add Project

**File**: `projects.html`

Add this block inside `<div class="project-grid">`:

```html
<div class="project-card">
  <img src="../assets/images/your-project.jpg" alt="Project Name" class="project-img">
  <button class="project-title">Project Name</button>
  <div class="panel">
    <p>Your detailed project description here...</p>
  </div>
</div>
```

**Add image**: `assets/images/your-project.jpg`
- Size: 800x600px recommended

---

## 🏆 Add Achievement

**File**: `_data/achievements.yml`

```yaml
- title: "Won Robocon 2025"
  description: "Our team secured 1st place in the national Robocon competition with an innovative autonomous robot design."
  year: "2025"
  link: "https://example.com/news"  # Optional
```

---

## ✍️ Write Blog Post

**Create**: `_posts/2025-12-07-my-awesome-post.md`

```markdown
---
layout: post
title: "My Awesome Robotics Project"
author: "Your Name"
date: 2025-12-07
---

## Introduction
Your content here...

## The Challenge
More content...

## Our Solution
Even more content...
```

---

## 🔗 Update Navigation Links

**File**: `_includes/header.html`

Find this section and modify:

```html
<div class="nav-menu" id="navMenu">
  <a href="{{ site.url }}/" class="nav-link">
    <span class="nav-icon">🏠</span>
    <span>Home</span>
  </a>
  <!-- Add your link here -->
  <a href="{{ site.url }}/new-page/" class="nav-link">
    <span class="nav-icon">✨</span>
    <span>New Page</span>
  </a>
</div>
```

---

## 📱 Update Social Media Links

**File**: `_includes/footer.html`

```html
<div class="footer-social">
  <!-- Instagram -->
  <a href="https://instagram.com/your_handle" target="_blank">
    <!-- SVG icon here -->
    <span>Instagram</span>
  </a>
  
  <!-- Add new social media -->
  <a href="https://twitter.com/your_handle" target="_blank">
    <svg><!-- Twitter icon --></svg>
    <span>Twitter</span>
  </a>
</div>
```

---

## 🎬 Change Animations

### Animation Speed
**File**: `css/modern-base.css`

```css
:root {
  --transition-fast: 0.2s;   /* Quick interactions */
  --transition-base: 0.3s;   /* Standard */
  --transition-slow: 0.5s;   /* Smooth */
}
```

### Disable Animations
**File**: `css/modern-base.css`

Add at the end:

```css
* {
  animation: none !important;
  transition: none !important;
}
```

---

## 📊 Update Statistics

**File**: `index.html`

Find the `hero-stats` section:

```html
<div class="hero-stats">
  <div class="stat-item">
    <div class="stat-value">50+</div>  <!-- Change number -->
    <div class="stat-label">Active Members</div>  <!-- Change label -->
  </div>
  <!-- More stats... -->
</div>
```

---

## 🌐 Change Website URL

**File**: `_config.yml`

```yaml
url: https://your-domain.com
title: Your Club Name
name: Your Club Name
```

---

## 📧 Update Contact Email

**File**: `_includes/footer.html`

Find:
```html
<a href="mailto:ibot_cfi@smail.iitm.ac.in">
```

Change to:
```html
<a href="mailto:your.email@example.com">
```

---

## 🎯 Add Call-to-Action Button

**Any page** - add this HTML:

```html
<div class="cta-section">
  <div class="container">
    <div class="cta-content">
      <h2>Join Our Next Workshop!</h2>
      <p>Learn robotics from experts and build your own robot.</p>
      <div class="cta-buttons">
        <a href="/register/" class="btn btn-primary">Register Now</a>
        <a href="/events/" class="btn btn-outline">View Schedule</a>
      </div>
    </div>
  </div>
</div>
```

---

## 🖼️ Optimize Images

### Before uploading images:

**Use online tools**:
- TinyPNG.com (compress)
- Squoosh.app (resize + compress)

**Recommended sizes**:
- Team photos: 800x800px
- Event banners: 1200x600px
- Project images: 800x600px
- Blog headers: 1200x630px

---

## 🔍 Add Google Analytics

**File**: `_includes/head.html`

Add before `</head>`:

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

---

## 🎨 Add Custom CSS

**Create**: `css/custom.css`

**Add to** `_includes/head.html`:
```html
<link rel="stylesheet" href="{{site.url}}/css/custom.css">
```

---

## 🐛 Debug Issues

### Clear Jekyll cache
```bash
bundle exec jekyll clean
bundle exec jekyll serve
```

### Check for errors
```bash
bundle exec jekyll build --verbose
```

### Browser console
1. Open browser
2. Press F12
3. Check Console tab for errors

---

## 💡 Quick Tips

1. **Always test locally** before committing
2. **Compress images** before uploading
3. **Use consistent naming** (lowercase-with-hyphens)
4. **Keep backups** of important files
5. **Document changes** in commit messages

---

## 🆘 Need Help?

- Check: [README.md](README.md)
- Check: [SETUP.md](SETUP.md)
- Email: ibot_cfi@smail.iitm.ac.in

---

**Happy Customizing! 🎨**
