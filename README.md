# How It Works 🛠

This document explains how the **React URL Shortener App** works.

---

 Core Functionality

1. **Enter a URL**
   - The user enters a long URL into the input field.
   - Optionally, the user can provide a **custom shortcode**.

2. **Generate Short URL**
   - The app creates a shortened URL.
   - If a custom shortcode is provided, it is used.  
   - Otherwise, a random string is generated.

3. **Save & Display**
   - The shortened URL is saved in the app’s local state (no backend).
   - All shortened URLs are displayed in a list with their original links.

4. **Analytics**
   - The app tracks the number of times each shortened link is clicked.
   - A stats section shows the **click count per URL**.

---

##  UI Details

- **Material UI** is used for input fields, buttons, and cards.
- **React Router** manages navigation between:
  - Home (`/`) → URL Shortener form and list.
  - Stats (`/stats`) → Analytics dashboard.

---

##  Workflow

1. User enters a long URL (and optional shortcode).  
2. App shortens it and displays the new link.  
3. When the shortened link is clicked, the app redirects to the original URL.  
4. Each click is counted and shown in the Stats page.

---

##  Tech Stack

- **React** (Frontend framework)
- **React Router DOM** (Page navigation)
- **Material UI** (UI components & styling)
- **Custom Logging Middleware** (Tracks app events)

---

✅ That’s it! The app is **fully client-side** and does not use a backend. All data is managed within the React state.
