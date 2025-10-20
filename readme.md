# Stage 1 Project — Multi-Page Application

This project builds upon the **Stage 0 Task**, expanding it into a multi-page web application.
It includes two new pages — a **Contact Us** page with form validation and an **About Me** page with reflective content.

---

## 📄 Pages Overview

### 1. Contact Us Page

A simple contact form that collects user details with validation and accessibility support.

#### **Required Fields**

* **Full Name** — `data-testid="test-contact-name"`
* **Email** — `data-testid="test-contact-email"`
* **Subject** — `data-testid="test-contact-subject"`
* **Message** — `data-testid="test-contact-message"`
* **Submit Button** — `data-testid="test-contact-submit"`

#### **Validation Rules**

* All fields are required.
* Email must be valid (e.g. `name@example.com`).
* Message must be at least **10 characters** long.
* On success, show a confirmation message — `data-testid="test-contact-success"`.
* Each error message should use:

  * Format: `data-testid="test-contact-error-<field>"`
  * Example: `data-testid="test-contact-error-email"`

#### **Accessibility**

* All inputs have `<label>` elements linked via the `for` attribute.
* Error messages use `aria-describedby` to connect to their inputs.
* The entire form is keyboard accessible.

---

### 2. About Me Page

A reflective page describing your thoughts and progress.

#### **Required Sections**

Each section should be inside a semantic `<section>` tag and have the listed `data-testid`.

* **Bio** — `data-testid="test-about-bio"`
* **Goals in this program** — `data-testid="test-about-goals"`
* **Areas of low confidence** — `data-testid="test-about-confidence"`
* **Note to future self** — `data-testid="test-about-future-note"`
* **Extra thoughts** — `data-testid="test-about-extra"`

#### **Structure**

* Wrap the page with `<main data-testid="test-about-page">`.
* Use semantic HTML (`<main>`, `<section>`, `<h2>`, `<h3>`, `<p>`).
* Ensure proper heading hierarchy and accessibility.

---

## ✅ Acceptance Criteria

### **Contact Us Page**

* All required fields exist with correct `data-testid`s.
* Validation prevents invalid submissions.
* Success message only appears after valid input.

### **About Me Page**

* All required sections exist with correct `data-testid`s.
* Uses semantic and accessible HTML.

---

## 🧠 Study Resources

* [Semantic HTML & Accessibility (MDN)](https://developer.mozilla.org/en-US/docs/Learn/Accessibility/HTML)
* [Form Validation in HTML/JS (MDN)](https://developer.mozilla.org/en-US/docs/Learn/Forms/Form_validation)
* [Accessibility for Forms (W3C)](https://www.w3.org/WAI/tutorials/forms/)
* [Responsive CSS Layouts (CSS-Tricks)](https://css-tricks.com/snippets/css/media-queries-for-standard-devices/)

