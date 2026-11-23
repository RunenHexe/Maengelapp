# 🛠️ Issue Reporter Web App

A lightweight, mobile-first web application designed for quick and seamless reporting of maintenance issues and building defects[cite: 1]. 

The app enables users to fill out a streamlined form in under a minute[cite: 1] and export the report as a high-resolution PNG image directly from their browser for easy sharing.

---

## 🌟 Key Features

* **Streamlined Single-Page Form:** Minimalistic input mask asking only for essential details to minimize entry effort[cite: 1].
* **Auto-Generated Metadata:** Automatically prefills the current timestamp and generates a unique Reference ID (UUID v4) for tracking[cite: 1].
* **Visual Urgency Selection:** Intuitive 3-stage symbol selection (🟢 Normal | 🟡 Important | 🔴 Urgent) for instant categorization[cite: 1].
* **Photo Upload & Preview:** Optional image attachment with an instant preview before generating the report[cite: 1].
* **Client-Side Image Export (PNG):** Uses `html2canvas` to render the report into a high-resolution, tamper-proof PNG image directly inside the browser.
* **Native Web Share Integration:** Shares the generated PNG directly via the device's native share menu (WhatsApp, Mail, Messenger, or local storage) with an automatic fallback download.
* **Progressive Web App (PWA):** Fully installable on smartphone home screens with offline capabilities via Service Worker caching[cite: 1].
* **100% Client-Side & Privacy-Focused:** Runs entirely in the browser without backends, databases, or stored contact details[cite: 1].

---

## 📱 Form Fields

1. **Reporter Name:** Name (and optional apartment number)[cite: 1].
2. **Date & Time:** Automatically prefilled with the current system timestamp[cite: 1].
3. **Urgency:** Symbol-based selection (🟢 Normal | 🟡 Important | 🔴 Urgent)[cite: 1].
4. **Description:** Multiline text field for defect details and location within the building[cite: 1].
5. **Photo:** Optional file upload for damage documentation[cite: 1].
6. **Reference ID:** Automatically generated UUID v4 in the background[cite: 1].

---

## 🚀 Deployment (GitHub Pages)

Since the application consists entirely of static client-side files, it can be hosted for free on **GitHub Pages**[cite: 1]:

1. Create a GitHub repository and upload the project files.
2. Navigate to **Settings → Pages** in your repository.
3. Under **Build and deployment**, set **Source** to *Deploy from a branch*.
4. Select the `main` (or `master`) branch and `/ (root)` folder, then save.
5. After a few minutes, the app will be live at `https://<username>.github.io/<repository-name>/`.

---

## 📁 File Structure

```text
.
├── index.html       # Main application layout, form, html2canvas & Web Share logic
├── manifest.json    # PWA configuration for home screen installation
├── sw.js            # Service worker for offline caching
├── icon-192.png     # App icon (192x192 px)
└── icon-512.png     # App icon (512x512 px)****
