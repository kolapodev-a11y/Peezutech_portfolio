# Kolapo Victor — React Portfolio

> **Zero npm install required!** This portfolio runs entirely in the browser via CDN.

## 📁 File Structure

```
portfolio-react/
├── index.html        ← Entry point
├── app.jsx           ← All React components (JSX compiled by Babel CDN)
├── style.css         ← All styles
├── images/           ← Copy your project images here
│   ├── land.jpg
│   ├── port.jpg
│   ├── ecomm.jpg
│   ├── blog.jpg
│   └── quiz.jpg
└── README.md
```

---

## 🚀 How to Run (No PC? No Problem!)

### Option A — Run in Browser (Simplest)
1. Extract the zip file
2. Place your project images in the `images/` folder
3. Double-click `index.html` to open in Chrome/Firefox/Edge
4. ✅ Done! No npm, no Node.js, no terminal needed.

> ⚠️ **Note:** Opening `.jsx` files directly may be blocked by some browsers due to CORS.
> Use **Option B** if you see a blank page.

### Option B — Use VS Code Live Server (Recommended)
1. Open the folder in VS Code
2. Install the **Live Server** extension
3. Right-click `index.html` → **Open with Live Server**
4. ✅ Runs at `http://127.0.0.1:5500`

### Option C — Deploy to Vercel (No PC Needed!)
1. Push all files to a GitHub repo
2. Go to [vercel.com](https://vercel.com) → New Project → Import from GitHub
3. No build settings needed — Vercel serves it as static HTML
4. ✅ Live URL in seconds!

### Option D — Use a Free Online Editor
- **[StackBlitz](https://stackblitz.com)** — Upload the files, run instantly
- **[CodeSandbox](https://codesandbox.io)** — Static HTML sandbox

---

## ✉️ Resend Setup (Contact Form)

This version sends your contact form email using **Resend** via a **Vercel Serverless Function** at `POST /api/contact`.

### 1) Create a Resend account + API key
- Create an API key in your Resend dashboard.

### 2) Add environment variables in Vercel
In **Vercel → Project → Settings → Environment Variables**, add:
- `RESEND_API_KEY` (required)
- `CONTACT_TO_EMAIL` (required) → where you want to receive the messages
- `CONTACT_FROM_EMAIL` (optional) → must be a verified sender in Resend. For testing you can use `onboarding@resend.dev`.
- `CONTACT_SUBJECT_PREFIX` (optional)

### 3) Deploy to Vercel
Because `Resend` runs server-side, the contact form **will not work if you open `index.html` directly with `file://`**.
Deploy to Vercel (or use a Node-based dev environment) to test.

### Resend API reference
See Resend’s “Send Email” endpoint docs.

---

## 🎨 Customization

All content is in `app.jsx` at the top — just edit the data arrays:

- **Skills:** Edit the `SKILLS` array
- **Projects:** Edit the `PROJECTS` array
- **Contact links:** Edit `CONTACT_METHODS` inside the `Contact` component
- **Colors:** Edit CSS variables in `style.css` (search for `#2563eb` = blue, `#7c3aed` = purple)

---

## 🌟 Features

- ⚛️ **100% React** (via CDN — no npm needed)
- 🎨 Dark theme with gradient accents
- ✨ Animated hero with typing effect
- 📱 Fully responsive (mobile-first)
- 🖱️ Scroll reveal animations
- 🔄 Hover effects on project cards
- 💌 Working contact form (EmailJS)
- ⬆️ Back-to-top button
- 🧭 Active nav link highlighting

---

Built with React (CDN) + CSS + ❤️ by Peezutech
