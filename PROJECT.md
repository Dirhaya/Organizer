# Tadween · Your semester, in order

A minimalist student planner for iPhone and Windows, styled with Ghars's warm beige, muted olive, rounded cards, and optional glass appearance.

## Current section: syllabus and PDF extraction

### Included
- Focused next-up card and a short upcoming list
- Manual dates for assignments, quizzes, tests, midterms, finals, registration windows, and deadlines
- Extracts text from selectable-text PDFs and .docx syllabuses in the browser
- Finds assessment and registration dates from nearby text and shows the source snippet for review
- Supports .ics, .csv, and simple .txt imports
- Date candidates can be deselected or corrected before adding
- Beige, white, black, and muted-glass themes
- Local browser storage, JSON backup/restore, offline app shell, and update checks
- GitHub Actions deployment workflow for GitHub Pages

### Extraction limits
- Scanned/image-only PDFs need OCR and are reported as unreadable; OCR is not included yet.
- Date detection uses text patterns and nearby keywords. It can miss dates or misclassify them; check every candidate and any inferred year.
- PDF.js and the Word reader load from a CDN. Files are read in the browser and are not uploaded by this feature.
- Data stays in one browser/device. Cross-device sync needs a backend or user-owned sync provider.
- The email connector is not connected to this app. Any mail filtering should use categories the student approves, with a review period and undo.

## Setup and publishing
1. In repository Settings → Pages, set the build source to GitHub Actions.
2. The workflow deploys on pushes to main.
3. Open the deployed URL in Safari on iPhone and choose Share → Add to Home Screen; on Windows use Edge/Chrome Install app.
4. For cross-device data, configure a sync backend before relying on both devices showing the same schedule.

## Data safety
Use Settings → Download backup before clearing site data or moving devices.
