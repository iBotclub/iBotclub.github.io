# 🤖 iBot Robotics Club - IIT Madras

[![Jekyll](https://img.shields.io/badge/Jekyll-4.0+-red.svg)](https://jekyllrb.com/)
[![License](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Website](https://img.shields.io/website?url=https%3A%2F%2Fibotclub.github.io)](https://ibotclub.github.io/)

> The official website for iBot Robotics Club, Indian Institute of Technology Madras - where innovation meets robotics.

**Live Site:** [ibotclub.github.io](https://ibotclub.github.io/)

---

## 🎨 Modern Design Features

This website has been completely redesigned with a modern, responsive, and engaging user experience:

### ✨ Key Features
- **🎯 Modern UI/UX**: Sleek, professional design with smooth animations
- **📱 Fully Responsive**: Optimized for all devices (desktop, tablet, mobile)
- **🚀 Performance**: Fast loading with optimized assets
- **♿ Accessible**: WCAG compliant with proper semantics and ARIA labels
- **🎭 Dark Theme**: Eye-friendly dark theme with accent colors
- **✅ Clean Code**: Modular CSS architecture with CSS variables

### 🎨 Design System
- **Primary Color**: `#ff1717` (iBot Red)
- **Typography**: Archivo Black (headings), Poppins (body)
- **Animations**: Smooth transitions and micro-interactions
- **Components**: Reusable cards, buttons, and sections

---

## 📁 Project Structure

```
iBotclub.github.io/
├── _config.yml              # Jekyll configuration
├── _layouts/                # Page layouts
│   ├── default.html        # Main layout template
│   ├── post.html           # Blog post layout
│   └── articles.html       # Articles layout
├── _includes/              # Reusable components
│   ├── header.html         # Modern navigation header
│   ├── footer.html         # Footer with social links
│   └── head.html           # HTML head section
├── _data/                  # Data files (YAML)
│   ├── core_25_26.yml      # Core team members
│   ├── cordis_25_26.yml    # Coordinators
│   ├── prev_cores.yml      # Previous heads
│   ├── achievements.yml    # Club achievements
│   └── events.yml          # Events timeline
├── _posts/                 # Blog posts (Markdown)
├── _articles/              # Technical articles
├── css/                    # Stylesheets
│   ├── modern-base.css     # Core design system
│   ├── home.css            # Homepage styles
│   ├── projects.css        # Projects page
│   ├── team.css            # Team page
│   ├── events.css          # Events page
│   ├── blog.css            # Blog page
│   ├── achievements.css    # Achievements page
│   └── notfound.css        # 404 page
├── assets/                 # Images, PDFs, etc.
├── index.html              # Homepage
├── projects.html           # Projects showcase
├── team.html               # Team members
├── events.html             # Events timeline
├── achievements.html       # Achievements
├── blog/                   # Blog index
└── 404.html                # Custom 404 page
```

---

## 🚀 Quick Start

### Prerequisites
- Ruby 2.7+
- Bundler
- Git

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/iBotclub/iBotclub.github.io.git
   cd iBotclub.github.io
   ```

2. **Install dependencies**
   ```bash
   gem install bundler
   bundle install --path vendor/bundle
   ```

3. **Run local development server**
   ```bash
   bundle exec jekyll serve --port 8080 --host 0.0.0.0
   ```

4. **View the site**
   Open your browser to `http://localhost:8080`

### Building for Production

Before committing changes, build the site:

```bash
bundle exec jekyll build
```

This generates the static site in the `docs/` directory.

---

## 📝 Content Management

### Adding Team Members

Edit `_data/core_25_26.yml` or `_data/cordis_25_26.yml`:

```yaml
- name: "Your Name"
  image: "your-photo.jpg"  # Place in assets/images/core_25_26/
  mob: "+91 XXXXXXXXXX"
  email: "your.email@example.com"
  instagram: "https://instagram.com/username"
  linkedin: "https://linkedin.com/in/username"
  github: "https://github.com/username"
```

### Adding Events

Edit `_data/events.yml`:

```yaml
- title: "Event Title"
  date: "Month Day, Year"
  description: "Event description here"
  image: "/assets/images/event/event-image.jpg"
  link: "/event/event-page.html"
  button_text: "Learn More"
  disabled: false
```

### Adding Blog Posts

Create a new file in `_posts/` with format `YYYY-MM-DD-title.md`:

```markdown
---
layout: post
title: "Your Post Title"
author: "Author Name"
date: 2025-MM-DD
---

Your blog content here in Markdown...
```

### Adding Projects

Edit `projects.html` to add new project cards.

### Adding Achievements

Edit `_data/achievements.yml`:

```yaml
- title: "Achievement Title"
  description: "Detailed description"
  year: "2025"
  link: "https://external-link.com"  # Optional
```

---

## 🎨 Customization

### Colors

Edit CSS variables in `css/modern-base.css`:

```css
:root {
  --primary-red: #ff1717;
  --bg-dark: #0a0e27;
  --text-primary: #ffffff;
  /* ... more variables */
}
```

### Typography

Change fonts in `css/modern-base.css`:

```css
:root {
  --font-display: 'Archivo Black', sans-serif;
  --font-body: 'Poppins', sans-serif;
}
```

---

## 🛠️ Technologies Used

- **Jekyll**: Static site generator
- **HTML5**: Semantic markup
- **CSS3**: Modern styling with variables, Grid, Flexbox
- **JavaScript**: Vanilla JS for interactions
- **Font Awesome**: Icon library
- **GitHub Pages**: Hosting

---

## 📱 Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Mobile browsers

---

## 🤝 Contributing

We welcome contributions! Here's how:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

### Contribution Guidelines

- Follow the existing code style
- Test on multiple devices/browsers
- Ensure all links work
- Optimize images before adding
- Write clear commit messages

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

---

## 👥 Team

Built with ❤️ by the iBot Club team at IIT Madras

**Maintainers:**
- iBot Core Team
- iBot Coordinators

---

## 📧 Contact

- **Email**: ibot_cfi@smail.iitm.ac.in
- **Instagram**: [@ibot_cfi_iitm](https://instagram.com/ibot_cfi_iitm)
- **Website**: [ibotclub.github.io](https://ibotclub.github.io)

---

## 🌟 Acknowledgments

- IIT Madras
- All iBot Club members past and present
- Open source community

---

**Last Updated**: December 2025

*For more information about iBot Club and our projects, visit our [website](https://ibotclub.github.io).*
