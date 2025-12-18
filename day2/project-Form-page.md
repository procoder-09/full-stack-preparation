# 🧩 Mini Project: Responsive Form Page

## 🎯 Project Goal

Build a **responsive, accessible form page** using **Semantic HTML + CSS**, applying everything you learned in:

* Semantic HTML
* Forms & Inputs
* Accessibility Basics
* Media Elements

This is a **portfolio-ready mini project** and a **common interview task**.

---

## 🧠 What You Will Learn

* Proper form structure
* Accessibility best practices (labels, focus, keyboard)
* Responsive layout using CSS
* Real-world form validation mindset

---

## 📄 Project Requirements

### Functional Requirements

* Name, Email, Password fields
* Gender (radio buttons)
* Skills (checkboxes)
* Profile photo upload
* Submit button

### Non‑Functional Requirements

* Responsive (mobile + desktop)
* Accessible (labels, focus, contrast)
* Semantic HTML only (no div abuse)

---

## 🗂️ Folder Structure

```
responsive-form/
├── index.html
├── style.css
└── README.md
```

---

## 🧱 HTML Structure (Semantic & Accessible)

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Responsive Form</title>
  <link rel="stylesheet" href="style.css" />
</head>
<body>

<header>
  <h1>User Registration</h1>
</header>

<main>
  <form>

    <section>
      <label for="name">Full Name</label>
      <input id="name" type="text" required />
    </section>

    <section>
      <label for="email">Email</label>
      <input id="email" type="email" required />
    </section>

    <section>
      <label for="password">Password</label>
      <input id="password" type="password" minlength="6" required />
    </section>

    <fieldset>
      <legend>Gender</legend>
      <label><input type="radio" name="gender" /> Male</label>
      <label><input type="radio" name="gender" /> Female</label>
    </fieldset>

    <fieldset>
      <legend>Skills</legend>
      <label><input type="checkbox" /> HTML</label>
      <label><input type="checkbox" /> CSS</label>
      <label><input type="checkbox" /> JavaScript</label>
    </fieldset>

    <section>
      <label for="photo">Profile Photo</label>
      <input id="photo" type="file" />
    </section>

    <button type="submit">Register</button>

  </form>
</main>

<footer>
  <p>© 2025</p>
</footer>

</body>
</html>
```

---

## 🎨 CSS (Responsive & Clean)

```css
* {
  box-sizing: border-box;
}

body {
  font-family: Arial, sans-serif;
  margin: 0;
  padding: 0;
}

header, footer {
  text-align: center;
  padding: 1rem;
  background: #222;
  color: #fff;
}

main {
  display: flex;
  justify-content: center;
  padding: 1rem;
}

form {
  width: 100%;
  max-width: 400px;
  display: flex;
  flex-direction: column;
  gap: 1rem;
}

label {
  font-weight: bold;
}

input, button {
  padding: 0.6rem;
}

button {
  background: #007bff;
  color: white;
  border: none;
  cursor: pointer;
}

button:hover {
  background: #0056b3;
}
```

---

## ♿ Accessibility Checklist

✅ Labels connected to inputs
✅ Keyboard navigation
✅ Proper input types
✅ Semantic elements

---

## 📱 Responsive Behavior

* Mobile → single column
* Desktop → centered card

---

## ❌ Common Mistakes (Avoid These)

* Missing labels
* Using only divs
* No `type` attributes
* Poor contrast

---

## 🎯 Interview Explanation (Say This)

> "I built a responsive, accessible form using semantic HTML and CSS. I focused on usability, keyboard navigation, and clean structure."

---

## ⭐ Bonus Improvements

* Add JS validation
* Add success message
* Store data in backend

---

## 🧠 Memory Summary

**Forms = Structure + Accessibility + Responsiveness**

---

If you want next, I can:

* 🔥 Add JavaScript validation
* 🔗 Connect to FastAPI backend
* 📄 Turn this into portfolio README
* 🎯 Provide interview Q&A
