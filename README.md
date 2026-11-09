# ScholarFlow · Learning & Research Studio

An automated academic workspace for shared course materials, source-matched evidence and reusable learning activities.

Upload once to prepare study notes, evidence cards and a reference record. Eight tools support misconception reflection, concept reconstruction, evidence mapping, assignment checking, method boundaries, replication outlines, version impact and quotation recovery.

## Deployment

This repository contains a standalone HTML/CSS/JavaScript frontend for GitHub Pages. Publish the `main` branch from `/ (root)`. Keep `.nojekyll` and the `assets/` folder together with `index.html`.

The frontend calls the existing ScholarFlow backend at https://scholarflow-studio-ak13.xiaoxiaosu.chatgpt.site for AI processing, shared records and original files. API keys stay on the backend. GitHub Pages does not run the backend or the private Google Drive script. The backend allows the `https://woainiaki13.github.io` and previously prepared `https://lucas-hkust.github.io` frontend origins.

To reuse an existing group, preserve its full `?room=...` invitation parameter when opening the Pages URL. Shared sources, completed learning packs and completed practice stay in the same cloud database. Drafts are specific to each browser and website origin. Anyone holding a group invitation link can read and contribute to that group.

## Files and processing

Supported uploads: PDF, PPTX, TXT and Markdown, up to 50 MB per file, 300 pages/slides and 500,000 extracted characters. Long documents are split automatically. Keep the page open until processing finishes; completed parts can be resumed on the same device. Scanned pages need OCR first. Images, complex charts and speaker notes are not interpreted automatically. Unknown citation fields and ambiguous page matches remain explicit.

The PDF.js and JSZip licenses are included in `assets/`.
