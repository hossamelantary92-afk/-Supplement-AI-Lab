# Supplement AI Lab — Phase 1

## Changes
- New responsive dark-mode research dashboard.
- Ten structured clinical information cards instead of unformatted text.
- `/api/analyze` now asks Gemini for JSON and returns `{ supplement, sections }`.
- No API key is stored in the browser or repository.
- Existing Vercel environment variable `GEMINI_API_KEY` and Gemini model are preserved.

## Deployment
1. Upload the updated `index.html` and `api/analyze.js` to the same paths in the existing GitHub repository.
2. Commit the changes and wait for Vercel deployment to show Ready.
3. Analyze `Vitamin D3` and check that the ten cards appear.

## Notes
- Gemini-generated content is not source-verified. A future phase will add evidence source validation.
- Copy, bilingual support, PDF export, history, and comparisons are future phases.
- For public deployment, add rate limits and abuse protection before significant traffic.
- An unrelated root-level `analyze.js` from the original repository was retained unchanged; the live endpoint is `api/analyze.js`.
