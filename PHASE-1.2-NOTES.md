# Supplement AI Lab — Phase 1.2

## Changes
- Request 1–2 short points per section rather than 2–4 to reduce generation time.
- Keep all ten clinical sections and tabbed presentation.
- Raise Gemini request timeout to 52 seconds and declare Vercel function maxDuration 60 seconds (subject to plan limits).
- Show a specific timeout error if the upstream call exceeds the deadline.
- Cache successful analyses in the current browser for seven days; repeat searches for the same name return immediately without calling Gemini. Clear browser site data to remove cache.
- Keep GEMINI_API_KEY on the server; no new secret or database needed.

## Deploy
Replace index.html and api/analyze.js in GitHub; commit and wait for Vercel Ready.

## Notes
Response time for new queries depends on Gemini and cannot be guaranteed. Cached answers can become stale; verify medical content and current evidence independently. The site still needs rate limiting and usage safeguards before public launch.
