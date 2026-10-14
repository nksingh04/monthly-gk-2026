# ज्ञानपथ · Gyanpath — Monthly GK 2026

Hindi-first bilingual static revision website: January–September 2026 only. 270 recall questions, 30 per month, 45 selected topics. No login, analytics, external runtime dependencies or backend.

Open `index.html` directly, or serve this directory with any static HTTP server. All asset paths are relative for GitHub Pages project hosting. The live site loads `data.js`; `data.json` is the maintainable source. After editing JSON, regenerate data.js as `window.GK_DATA = <JSON>;` and keep stable question IDs for saved progress.

Features: month navigation; Hindi/English switch; cross-month question, answer and topic search; revealable answers; saved questions; self-reported known/review progress; deterministic daily 10-question set; progress download. Daily practice uses the visitor’s local date. Progress is stored in localStorage on the same browser/origin and is not synchronized. The download is a backup record; this version has no import feature.

See [verification.md](verification.md) for source review scope and limits. Practice questions are neither MCQs nor authenticated past examination questions. This is independent selected-topic preparation, not official exam content or full syllabus coverage.

## Hosting

Publish the repository’s `main` branch root through GitHub Pages. `.nojekyll` disables Jekyll processing. No build command is required.

## Validation

JavaScript syntax and a simulated DOM interaction test cover all months, bilingual data, bookmarks, review state, progress, search, empty states, daily question selection, language switching, reload persistence and malformed storage. Browser-based visual QA was not performed under the session’s browser-control constraint.
