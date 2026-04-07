# DriveLog

A mobile-friendly web app for tracking vehicle expenses — fuel fill-ups, mileage reimbursements, maintenance, DEF fluid, and odometer readings. Built as a pure static site that runs entirely in your browser with optional Google Sheets cloud backup.

Works for any car, truck, or fleet vehicle. Supports both gasoline and diesel (with DEF tracking).

## Features

- **Fuel Tracker** — Log fill-ups with price/gallon, spend, volume, location, and odometer
- **Reimbursement Tracker** — Track mileage reimbursement claims and payment status
- **Maintenance Tracker** — Log services with costs and odometer readings
- **DEF Tracker** — Track diesel exhaust fluid purchases (diesel vehicles only)
- **Miles Tracker** — Log periodic odometer readings
- **Dashboard** — Interactive charts and KPIs (spend breakdown, MPG trends, reimbursement status)
- **Desktop Dashboard** — Open `dashboard.html` for a wider desktop-optimized view
- **Google Sheets Sync** — Optional cloud backup via Google Apps Script
- **Offline-first** — All data stored in browser localStorage, works without internet

## Quick Start

### Option 1: GitHub Pages (Recommended)

1. **Fork this repository** to your own GitHub account
2. Go to **Settings > Pages** in your fork
3. Set **Source** to `main` branch, folder `/ (root)`
4. Your app will be live at `https://YOUR-USERNAME.github.io/DriveLog/`
5. Open the app, go to **SETUP**, and enter your vehicle info

### Option 2: Run Locally

Just open `index.html` in any modern browser. No build tools, no server, no dependencies needed.

## Setup

Open the app and go to the **SETUP** tab to configure:

| Setting | Description |
|---------|-------------|
| **App Name** | Custom name shown in the header (e.g. "My Vehicle Log") |
| **Vehicle Name** | Your vehicle description (e.g. "2024 Toyota Tacoma") |
| **Fuel Type** | Diesel or Gasoline — diesel vehicles get the DEF tracker tab |
| **Last Odometer** | Starting odometer reading for auto-calculating miles driven |
| **Sheets URL** | Google Apps Script web app URL for cloud sync (optional) |

## Google Sheets Integration (Optional)

To sync your data to Google Sheets for backup or shared access:

1. Open `google_sheets_setup.html` for the full step-by-step guide
2. Create a Google Sheet with the required tabs
3. Deploy the included Apps Script as a web app
4. Paste the web app URL in the SETUP tab

## Files

| File | Description |
|------|-------------|
| `index.html` | Main tracker app (mobile-optimized) |
| `dashboard.html` | Desktop dashboard view (reads same localStorage data) |
| `google_sheets_setup.html` | Google Sheets integration setup guide |

## Tech Stack

- Pure HTML5 / CSS3 / Vanilla JavaScript
- [Chart.js](https://www.chartjs.org/) for dashboard visualizations
- Browser localStorage for persistence
- No frameworks, no build step, no server required

## License

MIT — Use it however you like.
