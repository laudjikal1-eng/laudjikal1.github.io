# Kontrak

Manage gigs, get paid — a contractor app for tracking clients, jobs, and invoices.

## What it is

Kontrak is a single-file, front-end prototype built with React (via CDN, no build
step required). It covers:

- **Onboarding** — quick intro + profile setup
- **Home** — daily overview: active jobs, outstanding balance, recent activity
- **Clients** — contact info and job history per client
- **Jobs** — job list with a stage tracker (Scheduled → In Progress → Review →
  Complete → Paid), photo tagging, file attachments, and notes
- **Pay** — invoice creation, PDF export, email drafts, and QR/Zelle payment collection
- **Settings** — profile, business/payment info, theme (light/dark), and text size

Responsive: a bottom tab bar on mobile, a sidebar workspace layout on desktop.

## Running it

No build step — just open `index.html` in a browser, or serve the folder with
any static file server:

```bash
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Stack

- React 18 + Babel Standalone (via CDN, in-browser JSX — no bundler)
- jsPDF for invoice PDF generation
- qrcode.js for Zelle payment QR codes
- Hand-rolled CSS design system (light/dark theme via CSS variables)

## Data

App data (clients, jobs, invoices, profile, and preferences) persists via the
`window.storage` API in supported environments. There is no backend — this is
a front-end prototype.

## Status

Prototype / work in progress.
