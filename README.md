# PRASTUTEE — sample NGO website

A responsive React + Vite + Tailwind CSS website concept. This is a standalone sample; no original source code is needed.

## Requirements
Node.js 18 or newer (Node.js 20+ recommended).

## Run locally
```bash
npm install
npm run dev
```
Open the local address printed in your terminal (usually http://localhost:5173).

## Build for Hostinger
```bash
npm run build
```
Upload the **contents** of the `dist` folder to `public_html` for static hosting.
For React Router deep links on Apache hosting, add this `.htaccess` file inside `public_html`:
```
<IfModule mod_rewrite.c>
RewriteEngine On
RewriteBase /
RewriteRule ^index\.html$ - [L]
RewriteCond %{REQUEST_FILENAME} !-f
RewriteCond %{REQUEST_FILENAME} !-d
RewriteRule . /index.html [L]
</IfModule>
```

## Customize
- Main components and page content: `src/main.jsx`
- Colors and typography: `tailwind.config.js` and `src/index.css`
- Logo: replace the leaf icon in `Header` with your official logo
- Images: replace the demo Unsplash image URLs with your own licensed photos
- Reports: add PDFs under `public/reports` and wire actual download links
- Donations: add the organization's verified payment link after approval
- Contact form: this demo opens the visitor's email application; it is **not** a backend contact form

## Important
All text, images, programs and statistics are **illustrative**. Confirm real organizational facts and content before publishing. No payment processing or data storage is included.
