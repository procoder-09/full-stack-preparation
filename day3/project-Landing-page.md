# Mini Project: Responsive Landing Page (Job‑Ready)

This mini project is designed exactly like a **real company frontend task**. You’ll practice **HTML, CSS, Flexbox, Grid, and Media Queries** together — the same skills used in day‑to‑day frontend / full‑stack jobs.

---

## 🎯 Project Goal

Build a **fully responsive landing page** that works perfectly on:

* Mobile
* Tablet
* Desktop

💼 **Real‑world usage**: Company websites, SaaS products, startup homepages, portfolios.

---

## 🧩 Sections to Build (Industry Standard)

1. **Header / Navbar**
2. **Hero Section**
3. **Features Section**
4. **Pricing Section**
5. **Footer**

---

## 🗂️ Folder Structure (Professional)

```
landing-page/
├── index.html
├── style.css
└── assets/
```

---

## 1️⃣ HTML Structure (Clean & Semantic)

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Landing Page</title>
  <link rel="stylesheet" href="style.css" />
</head>
<body>

  <!-- Header -->
  <header class="header">
    <div class="logo">MyProduct</div>
    <nav class="nav">
      <a href="#features">Features</a>
      <a href="#pricing">Pricing</a>
      <a href="#contact" class="btn">Get Started</a>
    </nav>
  </header>

  <!-- Hero -->
  <section class="hero">
    <div class="hero-content">
      <h1>Build Better Products Faster</h1>
      <p>Modern, scalable, and responsive UI for your business.</p>
      <button class="btn">Start Free Trial</button>
    </div>
  </section>

  <!-- Features -->
  <section id="features" class="features">
    <div class="feature">Fast Performance</div>
    <div class="feature">Secure Platform</div>
    <div class="feature">24/7 Support</div>
  </section>

  <!-- Pricing -->
  <section id="pricing" class="pricing">
    <div class="card">Basic</div>
    <div class="card">Pro</div>
    <div class="card">Enterprise</div>
  </section>

  <!-- Footer -->
  <footer class="footer">
    © 2025 MyProduct. All rights reserved.
  </footer>

</body>
</html>
```

---

## 2️⃣ CSS Styling (Flexbox + Grid + Media Queries)

```css
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font-family: Arial, sans-serif;
}

/* Header */
.header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 16px 32px;
  position: sticky;
  top: 0;
  background: #fff;
}

.nav a {
  margin-left: 16px;
  text-decoration: none;
}

.btn {
  padding: 8px 16px;
  background: #007bff;
  color: #fff;
  border-radius: 4px;
}

/* Hero */
.hero {
  display: flex;
  align-items: center;
  justify-content: center;
  height: 60vh;
  text-align: center;
}

/* Features (Grid) */
.features {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
  gap: 16px;
  padding: 32px;
}

.feature {
  padding: 24px;
  border: 1px solid #ddd;
  text-align: center;
}

/* Pricing (Flexbox) */
.pricing {
  display: flex;
  gap: 16px;
  padding: 32px;
}

.card {
  flex: 1;
  padding: 24px;
  border: 1px solid #ccc;
  text-align: center;
}

/* Footer */
.footer {
  text-align: center;
  padding: 16px;
  background: #f5f5f5;
}

/* Media Queries */
@media (max-width: 768px) {
  .nav {
    display: none;
  }

  .pricing {
    flex-direction: column;
  }
}
```

---

## 🧠 What You Learn (Job Skills)

| Skill         | How It’s Used         |
| ------------- | --------------------- |
| Flexbox       | Navbar, pricing cards |
| Grid          | Feature section       |
| Media Queries | Mobile responsiveness |
| box-sizing    | Layout stability      |
| Sticky header | Real UX behavior      |

---

## 💼 How to Explain This in an Interview

> “I built a responsive landing page using semantic HTML, Flexbox, Grid, and mobile‑first media queries. The layout adapts across devices, uses Grid for content sections and Flexbox for alignment‑based components like navbars and cards.”

---

## 🚀 Enhancements (Company‑Level)

* Add hamburger menu (JS)
* Add smooth scroll
* Add animations
* Convert to React components

---

## ✅ Final Summary

* This project matches **real frontend job tasks**
* Covers layout, responsiveness, and structure
* Perfect for **portfolio & interviews**

---

### Next Recommended Step

➡ **Convert this landing page into React components**
➡ Or **Deploy on Vercel / Netlify**

Tell me what you want to do next 👍
