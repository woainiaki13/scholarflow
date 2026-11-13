# ScholarFlow · Learning & Research Studio

An automated academic workspace for shared course materials, source-matched evidence and reusable learning activities.

Start with one material and one useful task: upload → automatic learning pack → explain one idea → inspect the original → save a revised understanding. The prominent **Start revising this lecture** button opens the real guided task; other tools remain available as optional actions. New runs use only the selected source and retain source, goal and explicit parent-run links. Drafts stay private. Completed results, saved reflections and student-entered study sessions use the existing shared cloud storage.

## Deployment

This repository contains a standalone HTML/CSS/JavaScript frontend for GitHub Pages. Pages uses the included **Publish ScholarFlow** GitHub Actions workflow; every push to `main` publishes the static website. Keep `.nojekyll` and the `assets/` folder together with `index.html`.

Live website: https://woainiaki13.github.io/scholarflow/

The frontend calls the existing ScholarFlow backend at https://scholarflow-studio-ak13.xiaoxiaosu.chatgpt.site for AI processing, shared records and original files. API keys stay on the backend. GitHub Pages does not run the backend or the private Google Drive script. The backend allows the `https://woainiaki13.github.io` and previously prepared `https://lucas-hkust.github.io` frontend origins.

To reuse an existing group, preserve its full `?room=...` invitation parameter when opening the Pages URL. Shared sources, completed learning packs and completed practice stay in the same cloud database. Drafts are specific to each browser and website origin. Anyone holding a group invitation link can read and contribute to that group.

## Files and processing

Supported uploads: PDF, PPTX, TXT and Markdown, up to 50 MB per file, 300 pages/slides and 500,000 extracted characters. Long documents are split automatically. Keep the page open until processing finishes; completed parts can be resumed on the same device. Scanned pages need OCR first. Images, complex charts and speaker notes are not interpreted automatically. Unknown citation fields and ambiguous page matches remain explicit.

The PDF.js and JSZip licenses are included in `assets/`.

## Real course demonstration

Watch the product film at https://woainiaki13.github.io/scholarflow/demo/. It uses an actual user-supplied 61-page finance lecture: four processing parts, 15 note sections, 19 source-matched evidence cards and a source-derived reference. The course title, author and semester year are retained; DOI and APA formatting remain unverified. The demo also explains source traceability, eight-tool reuse and shared cloud records.

## Task guide and factual use records

The first-use walkthrough follows a real revision task rather than introducing every tool. No model runs until the learner submits their own explanation. Study-session records accept the actual task, date, contributor, optional measured minutes and self-written issues or changes. Blank time fields remain unmeasured, not zero. Each saved session is a separate shared history record; unsubmitted session drafts stay local. Export factual records from **Record this study session**.

**Share group → Refresh display cache** reloads the interface and resets walkthrough progress while keeping sources, completed history, private drafts and unsent writes. This is a targeted interface refresh, not deletion of group data or all browser storage.

Evidence-card locations are rechecked against the full retained page map after all processing parts are merged. Saved packs with retained source maps are also rechecked on load. Repeated quotations show candidate pages instead of being labelled unique. A later audit found finance card C014 occurs on PDF pages 33 and 36; the earlier historical report's 16 unique assignments overstated global uniqueness. Original raw reports are retained; the supported full-document count is 15 single-page candidates and four multi-page candidates.

Technical details: [Chinese update note](docs/task-guide-update.md). These features record students' own experience; they do not generate final assessment analysis, establish learning gains or replace the course's GenAI declaration.

## Clearer first task

Start with **Check my understanding** for the selected lecture. Write an explanation, request feedback, open the original passage and save your own revision. **Study notes**, **Evidence cards** and **Source reference** open the corresponding part of the existing learning pack. Other tasks describe the input they need and the result they return.

The 14 November update moves this task into the first mobile screen, preserves source-derived question starters during navigation and gives each learning-pack output an exact destination. Existing group records, private drafts and model connections are retained. See [the update note](docs/usability-update.md).
