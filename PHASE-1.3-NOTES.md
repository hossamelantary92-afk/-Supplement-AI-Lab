# Phase 1.3 — Arabic explanations / English terminology

- Hero subtitle: Explore. Understand. Apply.
- Removed the requested AI-generated clinical verification sentence from the search hint; retained an educational disclaimer.
- Gemini instructed to return Arabic explanations with English clinical terminology, with concise JSON bullets.
- Prompt prefers ODS, NCCIH, Cochrane, PubMed-indexed research, and EFSA where relevant, but does **not** retrieve or verify live sources. No fabricated citations are permitted.
- Cache prefix changed to prevent old English answers being displayed.
- No changes to API key, model, or Vercel integration.

## Deployment
Replace `index.html` and `api/analyze.js` in the GitHub repository and commit. Wait for Vercel Ready.

## Important
This version does not provide source-grounded retrieval. Genuine source verification requires a separate evidence retrieval/validation workflow. AI-generated medical information must be checked against authoritative references before clinical use.
