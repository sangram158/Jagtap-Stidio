# Jagtap-Stidio

Demo portfolio + lightweight Canva-style editor.

## What this repo contains
- `index.html` — landing page + editor
- `styles.css` — site styles
- `script.js` — editor logic (add image, text, drag, export)
- `firebase.json` — hosting config
- GitHub Actions workflow for deploying to Firebase (see `.github/workflows`)

## Setup (quick)
1. Paste your Firebase config in `index.html` (the firebaseConfig object near top).
2. Enable **Firestore** and **Hosting** in Firebase console.
3. Create a Firebase Service Account JSON and add it to GitHub Secrets as `FIREBASE_SERVICE_ACCOUNT` (for CI deploy) — see the workflow file.
4. Push files — GitHub Actions will run and deploy to Firebase Hosting.

## Notes & next steps
- This is a starting point. If you want:
  - templates, layers, image cropping, or better text tools — we can add modules.
  - offline export improvements — we can add server-side rendering or more robust canvas drawing.
