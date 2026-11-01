# Tadween · Your semester, in order

A minimalist installable student planner for iPhone and Windows, styled with Ghars's warm beige, muted olive, rounded cards, and optional glass appearance.

## Current section: first working project build

### Included now
- Focused next-up card and a short upcoming list
- Manual dates for assignments, quizzes, tests, midterms, finals, registration windows, and deadlines
- Editable confirmation for dates imported from .ics, .csv, and simple .txt files
- Beige, white, black, and muted-glass themes
- Local browser storage and JSON backup/restore
- Offline app shell and automatic update checks when reopened online
- GitHub Actions deployment workflow for GitHub Pages

### Limits to address next
- Data currently stays in one browser/device; syncing iPhone and Windows needs a backend or a user-owned sync provider.
- PDF and Word syllabus extraction is not implemented; use .ics, .csv, or text for imports for now.
- The email connector is not connected to this app. Mail filtering should use categories the student approves, with a review period and undo, before any automatic archive or movement.

## Setup and publishing
1. In the repository Settings → Pages, set the build source to GitHub Actions.
2. The workflow deploys on pushes to main.
3. After deployment, open the Pages URL in Safari on iPhone and choose Share → Add to Home Screen; on Windows, use Edge/Chrome Install app.
4. For cross-device data, choose and configure a sync backend before relying on both devices showing the same schedule.

## Data safety
Never rely on local browser data as the only copy. Use Settings → Download backup before clearing site data or moving devices.
