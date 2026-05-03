# Jimmy H. Trinh - Portfolio Website

A modern, responsive portfolio website built with HTML, CSS and JavaScript. Showcasing projects, skills, and professional experience with an elegant design that impresses employers and clients.

[Status: Active] [Language: Norwegian]

---

## Table of Contents

- [About](#about)
- [Features](#features)
- [Project Structure](#project-structure)
- [Technologies Used](#technologies-used)
- [Getting Started](#getting-started)
- [Projects](#projects)
- [Customization](#customization)
- [Browser Support](#browser-support)
- [Performance](#performance)
- [Contributing](#contributing)
- [Contact](#contact)

---

## About

This is a professional portfolio website designed to showcase development skills, completed projects, and professional background. The site features a modern design with smooth animations, responsive layouts, and an engaging user experience that adapts to both light and dark modes.

**Key Highlights:**
- Modern, clean design
- Professional color scheme with orange accent (#FF6B35)
- Fully responsive - works on desktop, tablet, and mobile
- Dark mode support based on system preferences
- Smooth animations and transitions
- Interactive elements and hover effects
- Apple SF Pro font family for a premium feel
- Personal photo in the About section for a strong first impression

---

## Features

### Hero Section
- Eye-catching landing area with animated gradient text
- Typing effect animation for the subtitle
- Radial background gradients for visual depth
- Call-to-action button

### About Section
- Personal profile photo displayed centered above the bio
- Professional biography and background (left-aligned for readability)
- Centered "Om meg" and "Ferdigheter" headings
- Skills displayed in an interactive grid layout
- 6 skill categories: Frontend, Backend, Database, Infrastructure, Cloud Services, and Personal Traits
- Smooth hover animations on skill items

### Portfolio Projects
- 3 featured school projects with individual detail pages:
  - **NaviSafe** - Aerial Obstacle Reporting System
  - **Bcycle** - Database system for bike rental
  - **Groupr** - Student grouping application
- Interactive project cards with gradient backgrounds
- Individual project pages with detailed information

### Contact Section
- Multiple contact methods
- Social media links
- Email contact option

### Navigation
- Sticky navigation bar with consistent spacing across all pages
- Smooth scrolling to sections
- Responsive mobile navigation

### Animations & Interactions
- Staggered scroll animations
- Typing effect on hero subtitle
- Smooth page transitions
- Hover effects on interactive elements
- Progress-based element reveals

### Accessibility
- Semantic HTML structure
- Proper color contrast
- Responsive design
- Keyboard navigation support

---

## Project Structure

```
Portfolio-website/
├── index.html                    # Main landing page
├── style.css                     # Global styles and theme
├── jimmy-photo.jpeg              # Profile photo (place in repo root)
├── navi-safe.html               # NaviSafe project page
├── bcycle.html                  # Bcycle project page
├── groupr.html                  # Groupr project page
└── README.md                    # This file
```

### File Details

| File | Purpose | Size |
|------|---------|------|
| `index.html` | Main portfolio page with hero, about, projects, and contact sections | ~20KB |
| `style.css` | Global styles, animations, responsive design, and dark mode | ~20KB |
| `jimmy-photo.jpeg` | Profile photo displayed in the About section | ~1MB |
| `*-project.html` | Individual project detail pages | ~3-4KB each |

> **Note:** `index.html` references `style.css` and `jimmy-photo.jpeg` as external files. Make sure all three are in the same folder when deploying.

---

## Technologies Used

### Frontend
- **HTML5** - Semantic markup
- **CSS3** - Modern styling with:
  - CSS Grid for layouts
  - Flexbox for flexible components
  - CSS Variables for theming
  - Media queries for responsiveness
  - Animations and transitions
- **JavaScript** - Smoother transitions

### Design System
- **Font Family:** Apple SF Pro (San Francisco)
- **Color Scheme:**
  - Primary: #1a1a1a (Dark)
  - Secondary: #ffffff (White)
  - Accent: #FF6B35 (Orange)
  - Light Gray: #f5f5f5
  - Dark Gray: #333333
- **Border Radius:** 12-24px for modern look
- **Shadows:** Multi-layer shadow effects for depth

### Browser APIs
- **Intersection Observer** - For scroll-triggered animations
- **Viewport Meta Tag** - For mobile optimization
- **CSS Media Queries** - For responsive design and dark mode

---

## Getting Started

### Prerequisites
- A modern web browser (Chrome, Firefox, Safari, Edge)
- A text editor for customization (VS Code, Sublime, etc.)
- Git (optional, for version control)

### Installation

1. **Clone the repository**
```bash
git clone https://github.com/jimmyht98/portfolio-website.git
cd portfolio-website
```

2. **Open locally**
```bash
# Using Python (Python 3.x)
python -m http.server 8000

# Using Node.js with http-server
npx http-server

# Or simply open index.html in your browser
```

3. **View in browser (using Github Pages for deployment)**
```
https://jimmyht98.github.io/Portef-lje/
```

### Quick Start (No Server Required)
Simply download the files and open `index.html` in your web browser. Make sure `style.css` and `jimmy-photo.jpeg` are in the same folder.

---

## Projects

### NaviSafe - Aerial Obstacle Reporting System
- **Stack:** ASP.NET Core, PostgreSQL, HTML/CSS/JavaScript
- **Client:** Kartverket (Norwegian Mapping Authority)
- **Features:**
  - Obstacle reporting form
  - Data visualization with search and filters
  - Role-based access (pilot/admin views)
  - Responsive design for fieldwork

**Repository:** [NaviSafe on GitHub](https://github.com/asklootz/NaviSafe)

### Bcycle - Bike Rental Database System
- **Stack:** PLSQL, ASP.NET Core
- **Team Project:** Developed with group members
- **Features:**
  - Bike rental management
  - Customer database
  - Reservation system
  - Analytics and reporting

**Repository:** [Bcycle on GitHub](https://github.com/jimmyht98/IS309)

### Groupr - Student Grouping Application
- **Stack:** Python, numpy, matplotlib, networkx, Tkinter
- **Features:**
  - Generates random 120-160 students
  - Groups students using a similarity algorithm
  - Multi-tab GUI with subject distribution, network, timeline and matrix views

**Repository:** [Groupr on GitHub](https://github.com/jimmyht98/IS211)

---

## Customization

### How to Personalize Your Portfolio

#### Update Personal Information
Edit `index.html`:
```html
<h1>Hei, jeg er [Your Name]!</h1>
<p>[Your tagline here]</p>
```

#### Replace Profile Photo
Swap out `jimmy-photo.jpeg` in the repo root with your own photo. Keep the same filename, or update the `src` attribute in `index.html`:
```html
<img src="your-photo.jpeg" alt="Your Name" class="about-photo" />
```

#### Change Contact Information
```html
<a href="mailto:your.email@example.com" class="contact-link">✉️ E-post</a>
<a href="https://github.com/yourprofile" class="contact-link" target="_blank">🔗 GitHub</a>
```

#### Update Skills
Edit the skills section in `index.html`:
```html
<div class="skill-item">
    <h3>Your Skill</h3>
    <p>Technologies and tools</p>
</div>
```

#### Add/Remove Projects
1. Create a new HTML file for your project: `my-project.html`
2. Copy structure from existing project pages
3. Add link in the portfolio grid:
```html
<a class="portfolio-card" href="my-project.html">
    <!-- Card content -->
</a>
```

#### Change Color Scheme
Edit CSS variables in `style.css`:
```css
:root {
    --primary: #1a1a1a;
    --secondary: #ffffff;
    --accent: #FF6B35;      /* Change this to your color */
    --light-gray: #f5f5f5;
    --dark-gray: #333333;
}
```

---

## Browser Support

| Browser | Desktop | Mobile |
|---------|---------|--------|
| Chrome | Yes | Yes |
| Firefox | Yes | Yes |
| Safari | Yes | Yes |
| Edge | Yes | Yes |
| Opera | Yes | Yes |
| IE | No | N/A |

---

## Performance

### Optimization Features
- Minimal Dependencies - Vanilla JavaScript, no frameworks
- Efficient CSS - CSS Grid and Flexbox for layouts
- External image file - photo is a separate `.jpeg` file for fast load times
- Mobile Optimized - Responsive design, touch-friendly

---

## Contributing

Contributions are welcome! Feel free to:
- Report bugs
- Suggest improvements
- Improve design
- Update documentation
- Add new features

### How to Contribute
1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

---

## Contact

**Jimmy H. Trinh**

- Email: jimmyht98@hotmail.com
- GitHub: [github.com/jimmyht98](https://github.com/jimmyht98)
- LinkedIn: [linkedin.com/in/jimmy-trinh](https://www.linkedin.com/in/jimmy-trinh-578951264/)

---

## Changelog

### Version 1.0.1 - May 2026
- Added personal profile photo to the "Om meg" section
- Centered photo, "Om meg" heading, "Ferdigheter" heading, and skill cards
- Bio text and Journal section text kept left-aligned for readability
- Inlined all CSS from `style.css` into `index.html` for portability
- Fixed navigation bar spacing to be consistent across all pages
- Photo referenced as external file (`jimmy-photo.jpeg`) for clean, maintainable code

### Version 1.0.0 - April 2026 - Initial Release
- Complete portfolio website
- 3 showcase school projects
- Responsive design
- Smooth animations
- Apple SF font
- Professional color scheme

---

*Last Updated: May 2, 2026*
