# Medical Lab History PWA

Prototype Android-friendly progressive web app for personal lab tracking.

## Features
- Import selectable-text PDF; review, edit, exclude, and confirm candidate results.
- Manual entry, historical charts, latest results, configurable reference ranges and high/low flags.
- Delete checkup records.
- Manual JSON backup and restore.
- Browser-local storage and service-worker caching for the app shell.

## Important limitations
PDF extraction uses general text heuristics and can pair a wrong number with a label. Always compare every candidate against the original report before saving. A template-specific extraction mapping should be validated against sample reports before relying on it. Scanned/image-only PDFs are unsupported. PDF.js loads from a CDN, so first-time PDF extraction needs internet; this package does not bundle the PDF.js library itself. Browser data may be cleared; export backups regularly. Reference ranges are editable examples, not universal clinical thresholds.

## Install on Android
Host these files on an HTTPS site, open it in Chrome, then select **Install app** or **Add to Home screen**. Opening index.html directly from a file manager may not enable PWA/service-worker behavior.
