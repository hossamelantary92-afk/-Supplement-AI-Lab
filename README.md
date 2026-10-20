# Supplement AI Lab

A beginner-friendly HTML/CSS/JS frontend with a Vercel serverless API route calling Gemini.

## Deploy
1. Push this folder to a GitHub repository. Never commit your real API key.
2. Import the repository at https://vercel.com/new . Use framework preset **Other** and root directory containing `index.html` and `api/`.
3. In Vercel Project Settings → Environment Variables, add `GEMINI_API_KEY` with your real key from Google AI Studio. Do **not** use `VITE_` or `NEXT_PUBLIC_` prefixes.
4. Deploy (or redeploy after setting the variable), then test the site.

## Local development
Install Node.js 20+ and run `npx vercel dev` in the project directory. Set the environment variable in Vercel and use Vercel CLI to pull development variables when appropriate. Do not commit `.env` files.

## Important security notes
- The server-side key is not sent to the browser.
- **This is a teaching demo, not a production-hardened public AI service.** Before a public launch add authentication or abuse prevention, rate limiting, spending quotas/alerts, and request monitoring. Otherwise strangers can consume your API quota through the public endpoint.
- Gemini output can be incorrect; verify medical claims independently.
- The example model is `gemini-2.5-flash`; availability and pricing may change.
