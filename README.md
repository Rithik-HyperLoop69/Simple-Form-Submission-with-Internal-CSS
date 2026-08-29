# Information Form Submission

🔗 **Live Demo:** [simple-form-submission-with-interna.vercel.app](https://simple-form-submission-with-interna.vercel.app/)

A stylish, space-themed HTML form that collects user information and sends it directly to an email address via [FormSubmit](https://formsubmit.co/).

---

## Overview

This is a single-page static web project featuring a glassmorphism-styled form set against a No Man's Sky game wallpaper background. It requires no backend — form submissions are handled entirely by the FormSubmit service.

---

## Features

- **Email delivery** — Submissions are sent directly to `silentdude689@gmail.com` via FormSubmit (no backend needed)
- **Spam protection** — CAPTCHA is disabled for a smoother user experience (configurable)
- **Glassmorphism UI** — Frosted-glass form card with a cinematic space background
- **Custom typography** — Google Fonts: Zen Dots, Caveat Brush, Patrick Hand, Playwrite GB J, Orbitron, Exo 2
- **Responsive layout** — Centered form capped at 600px width
- **Branded footer** — RITHIK.DEV footer with version badge and copyright

---

## Project Structure

```
project/
└── index.html       # The entire project — HTML, CSS, and form logic in one file
```

No external JS files, no build tools, no dependencies beyond Google Fonts.

---

## Form Fields

| Field | Type | Required |
|---|---|---|
| Username | Text | Yes |
| Phone Number | Number | Yes |
| Email | Email | Yes |
| Gender | Radio (Male / Female / Other) | Yes |
| Comment | Textarea | No |
| Newsletter Subscription | Checkbox | No |

---

## How to Use

### 1. Clone or Download
Download `index.html` or copy the source code into a new file.

### 2. Open in Browser
Simply open `index.html` in any modern browser — no server required for viewing.

### 3. Deploy
Upload `index.html` to any static hosting platform:

- **GitHub Pages** — Push to a repo and enable Pages in settings
- **Netlify** — Drag and drop the file at [netlify.com/drop](https://app.netlify.com/drop)
- **Vercel** *(currently deployed)* — [simple-form-submission-with-interna.vercel.app](https://simple-form-submission-with-interna.vercel.app/)

### 4. First Submission Activation
FormSubmit requires a **one-time email confirmation** the first time a form is submitted to a new email address. Check `silentdude689@gmail.com` after the first submission and click the confirmation link.

---

## Configuration

To change the recipient email, update the `action` attribute in the `<form>` tag:

```html
<form action="https://formsubmit.co/your@email.com" method="POST">
```

To re-enable CAPTCHA, change the hidden input:

```html
<input type="hidden" name="_captcha" value="true">
```

Other useful FormSubmit options you can add as hidden inputs:

```html
<!-- Redirect after submission -->
<input type="hidden" name="_next" value="https://yoursite.com/thankyou.html">

<!-- Custom email subject -->
<input type="hidden" name="_subject" value="New Form Submission!">
```

---

## Design Details

| Property | Value |
|---|---|
| Background | No Man's Sky wallpaper (external URL) |
| Form style | Glassmorphism (`backdrop-filter: blur(20px)`) |
| Primary font | Zen Dots (labels), Caveat Brush (inputs) |
| Accent color | `#3a9bdc` (blue) |
| Button | `#007BFF` → `#0f335a` on hover |
| Input background | `#0f335a` (dark navy) |

---

## Technologies Used

- **HTML5** — Semantic structure
- **CSS3** — Styling, backdrop filters, Google Fonts, transitions
- **FormSubmit** — Email delivery service (free, no account needed)
- **Google Fonts** — Custom typefaces loaded via CDN

---

## 📜 License

© 2026 **Rithik** — All rights reserved.  
*Information Form v1.0*
