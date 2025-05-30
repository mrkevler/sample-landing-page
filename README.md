# Sample Landing Page by mrKevler 💫

**Repository:** [github.com/mrkevler/sample-landing-page](https://github.com/mrkevler/sample-landing-page)

**Demo** 🌐 [mrkevler.github.io/sample-landing-page](https://mrkevler.github.io/sample-landing-page)

![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white) ![CSS3](https://img.shields.io/badge/CSS3-1572B6?logo=css3&logoColor=white) ![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black)  
![GitHub](https://img.shields.io/badge/GitHub-mrkevler-green) ![License](https://img.shields.io/badge/License-CC%20BY--NC-blue)  
![Repo Size](https://img.shields.io/github/repo-size/your-username/html-web-pages) ![Last Commit](https://img.shields.io/github/last-commit/your-username/html-web-pages)  
[![Buy Me a Coffee](https://img.shields.io/badge/Support-Buy%20Me%20a%20Coffee-yellow)](https://buymeacoffee.com/mrkevler)

## 🔍 Table of Contents

- [Sample Landing Page by mrKevler 💫](#sample-landing-page-by-mrkevler-)
  - [🔍 Table of Contents](#-table-of-contents)
  - [🚀 Project Overview ](#-project-overview-)
  - [✨ Concept ](#-concept-)
  - [🌟 Key Features ](#-key-features-)
  - [💫 Page Structure ](#-page-structure-)
    - [Landing Page Features](#landing-page-features)
    - [Form Pages](#form-pages)
  - [🛠️ Technologies Used ](#️-technologies-used-)
  - [💻 Code Showcase ](#-code-showcase-)
    - [Core CSS Patterns and Why They're Used](#core-css-patterns-and-why-theyre-used)
    - [Advanced Layout Features](#advanced-layout-features)
  - [🏗️ Project Structure ](#️-project-structure-)
  - [🚀 HowTo Use ](#-howto-use-)
    - [Page Highlights:](#page-highlights)

---

## 🚀 Project Overview <a name="-project-overview"></a>

This is a sample landing page built with HTML, CSS and JavaScript 💫  
Built with semantic HTML5, modern CSS3 and vanilla JavaScript to showcase professional web development patterns 🎨

This tutorial is perfect for learning modern web design and responsive layout techniques 🎓

Enjoy coding! ✌️  
[mrKevler](https://github.com/mrkevler)

---

## ✨ Concept <a name="-concept"></a>

This project demonstrates four core web development skills:

1. **Semantic HTML5** structure with accessibility and form validation
2. **Advanced CSS3** styling with gradients, animations and responsive design
3. **Modern Layout** techniques with CSS Grid and Flexbox
4. **Professional UX patterns** with smooth transitions and interactive elements

Key learning objectives:

- Vertical navigation with smooth scrolling
- Responsive grid layouts for feature cards
- Form design with custom styling and validation
- CSS custom properties for consistent theming
- Mobile-first responsive design approach

---

## 🌟 Key Features <a name="-key-features"></a>

Professional HTML5, CSS3 and JavaScript implementation  
Vertical sidebar navigation with smooth scrolling  
Responsive grid layout for feature presentation  
Custom form styling with validation patterns  
Modern gradient backgrounds and hover effects  
Mobile-optimized design with collapsible navigation

---

## 💫 Page Structure <a name="-page-structure"></a>

### Landing Page Features

| Section           | Implementation                            |
| ----------------- | ----------------------------------------- |
| **Hero Section**  | Gradient background with statistics       |
| **Features Grid** | 3 column responsive layout with cards     |
| **Testimonials**  | Customer feedback with profile images     |
| **About Section** | Two column layout with team photo         |
| **Navigation**    | Fixed vertical sidebar with smooth scroll |

### Form Pages

- **Signup Page** - User registration
- **Signin Page** - User authentication

---

## 🛠️ Technologies Used <a name="-technologies-used"></a>

| Technology            | Implementation                      |
| --------------------- | ----------------------------------- |
| **HTML5**             | Semantic markup, form validation    |
| **CSS3**              | Custom properties, Grid, Flexbox    |
| **JavaScript**        | DOM manipulation, smooth scrolling  |
| **Responsive Design** | Mobile-first, flexible grid layouts |

---

## 💻 Code Showcase <a name="-code-showcase"></a>

### Core CSS Patterns and Why They're Used

```css
/* 1. CSS custom properties for consistency */
:root {
  --primary-blue: #1e88e5;
  --turquoise: #4dd0e1;
  --mint: #b2dfdb;
  --cream: #f5e6d3;
}

/* 2. Vertical navigation with fixed positioning */
nav {
  width: 250px;
  background: linear-gradient(145deg, var(--cream), var(--mint));
  position: fixed;
  height: 100vh;
}

/* 3. Responsive grid layouts */
.features-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 30px;
}

/* 4. Smooth hover transformations */
.feature-card:hover {
  transform: translateY(-10px);
  box-shadow: 0 25px 60px rgba(30, 136, 229, 0.18);
}
```

### Advanced Layout Features

```javascript
// 1. Smooth scrolling navigation
document.querySelectorAll('a[href^="#"]').forEach((anchor) => {
  anchor.addEventListener("click", function (e) {
    e.preventDefault();
    const target = document.querySelector(this.getAttribute("href"));
    if (target) {
      target.scrollIntoView({
        behavior: "smooth",
        block: "start",
      });
    }
  });
});

// 2. Dynamic year updating
document.addEventListener("DOMContentLoaded", function () {
  const currentYear = new Date().getFullYear();
  const yearElement = document.getElementById("currentYear");
  if (yearElement) {
    yearElement.textContent = currentYear;
  }
});

// 3. Active navigation highlighting
window.addEventListener("scroll", () => {
  const sections = document.querySelectorAll("section[id]");
  const navLinks = document.querySelectorAll(".nav-menu a");

  let current = "";
  sections.forEach((section) => {
    const sectionTop = section.offsetTop;
    if (pageYOffset >= sectionTop - 200) {
      current = section.getAttribute("id");
    }
  });

  navLinks.forEach((link) => {
    link.classList.remove("active");
    if (link.getAttribute("href") === `#${current}`) {
      link.classList.add("active");
    }
  });
});
```

---

## 🏗️ Project Structure <a name="-project-structure"></a>

```
html-web-pages/
├── index.html
├── sign-up.html
├── sign-in.html
├── README.md
└── assets/
    ├── css/
    │   └── style.css
    ├── script/
    │   └── script.js
    └── image/
        ├── logo.svg
        ├── bg.svg
        ├── coding.png
        ├── team.svg
        └── ok.svg
```

---

## 🚀 HowTo Use <a name="-usage"></a>

1. Clone the repo:

```bash
git clone https://github.com/mrkevler/sample-landing-page.git
```

2. Open index.html in any browser

3. Navigate through features:
   - Use vertical navigation menu
   - Test responsive design on mobile
   - Fill out signup/signin forms
   - Experience smooth scrolling

**Sample landing page design** 🎨  
**Responsive layout with modern CSS Grid** 📱  
**Clone, customize, and deploy in minutes!** 🚀

### Page Highlights:

- **Landing Page** - Hero section, features grid, testimonials, about
- **Sign Up** - User registration form with coding illustration
- **Sign In** - Authentication form with consistent styling

**Sample Landing Page by mrKevler** showcasing modern web development patterns for educational platforms 📚

---

[![Buy Me a Coffee](https://img.shields.io/badge/Buy%20Me%20a%20Coffee-FF8000?style=for-the-badge&logo=buymeacoffee&logoColor=white)](https://www.buymeacoffee.com/mrkevler)

Crafted with ♥ by [mrKevler](https://github.com/mrkevler)
