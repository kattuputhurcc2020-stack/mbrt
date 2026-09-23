Quality Control & Lab Management Portal 🥛🔬

A lightweight, mobile-optimized Progressive Web Application (PWA) designed for real-time quality control, transport route MBRT monitoring, and raw milk spoilage tracking.
✨ Key Features

    MBRT Transport Route Tracking:

        Route-wise MBRT test logging with dynamic Hours & Minutes formatting (X hr Y min).

        Auto-fetched Previous MBRT: Instantly pulls the last recorded value for each specific transport route.

        Live Difference Calculation: Automatically computes the quality improvement or decrease with dynamic indicators (▲ / ▼).

        Automated Quality Statement Pills: Categorizes route performance live (Above 1 hr, Below or Equal to 1 hr, Below or Equal to 30 min).

    Raw Milk Spoilage & Adulteration Management:

        Supports comprehensive test types: Warning, Cob positive, Alcohol 65%, Sugar, Salt, and Urea.

        Smart 30-Day Dynamic Remarks: Automatically tracks prior 30-day shift occurrences for any given center code (e.g., COB POSITIVE 1, ALCOHOL 65% 2) or displays NIL.

        Flexible Warning Quantities: Allows Warning entries without requiring milk volume quantities.

    Desktop-Grade Report Synthesis & Export Engine:

        Generates clean, formatted summary tables filtered by Single Date & Shift or Date Ranges.

        HD JPEG Snapshot Export: Uses html2canvas to render high-resolution downloadable image snapshots of reports.

        Excel Spreadsheet Export: Uses SheetJS (xlsx) to export detailed tabular data formatted for spreadsheet software.

    Robust Dual-Storage & Cloud Synchronization:

        Zero-Lag Local Storage: All records are instantly saved locally to browser storage for offline reliability.

        Google Sheets & Drive Backend: Seamlessly syncs entries and pulls historical logs using a deployed Google Apps Script Web App.

        JSON Backup & Restore: Built-in admin controls to export complete local storage backups as .json files or restore them instantly.

🛠️ Technology Stack

    Frontend: HTML5, Tailwind CSS (CDN), Vanilla JavaScript (ES6+).

    Icons & Fonts: FontAwesome 6.4.0, Plus Jakarta Sans.

    Export Libraries: SheetJS (xlsx.full.min.js), html2canvas (html2canvas.min.js).

    Backend Integration: Google Apps Script (doGet / doPost Web App endpoints), Google Sheets API.

🚀 Quick Start Guide

    Clone or download this repository.

    Open index.html in any modern web browser or host it on GitHub Pages, Vercel, or Netlify.

    (Optional) To connect your live Google Sheet backend:

        Open your Google Sheet > Extensions > Apps Script.

        Paste your backend deployment script and copy your Web App URL.

        Replace const SCRIPT_URL = "..." inside index.html with your deployed Web App URL.

📂 Project Structure
Plaintext

├── index.html                  # Complete single-file PWA frontend application
├── Code.gs                     # Google Apps Script backend controller
├── Spoilage_August_2026.csv    # Monthly historical CSV template
└── README.md                   # Project documentation

📱 Mobile-First Navigation

The portal features a docked floating bottom navigation bar designed for rapid shift-change data entry on mobile devices and tablets:

    MBRT: Route MBRT test logger and live quality statement pills.

    SPOILAGE: Center spoilage, adulteration, and auto-calculated 30-day remark tracker.

    REPORT: Multi-mode report generator with instant JPEG & Excel download buttons.

    ADMIN: JSON backup exporter, JSON backup restorer, and factory reset tools.

    SYNC: Manual cloud synchronization trigger with animated status spinners.

📄 License

This project is released under the MIT License.
