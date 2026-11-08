# Football IQ Dashboard — starter frontend

This is the first frontend foundation for your existing Cloudflare Worker backend.

## Run locally
1. Extract the ZIP.
2. Open `index.html` in Chrome.
3. The page requests fixtures from:
   `https://football-iq-api.nakalemasalima250.workers.dev/api/fixtures?date=YYYY-MM-DD`

If the browser blocks the request, check the Worker CORS response for your deployed frontend origin.

## Deploy on Cloudflare Pages
1. Create a GitHub repository and upload `index.html`.
2. In Cloudflare, open Workers & Pages → Create → Pages → Connect to Git.
3. Select the repository.
4. Framework preset: None.
5. Build command: leave blank.
6. Build output directory: `/` (or the repository root, depending on the Pages setup screen).
7. Deploy.

## Current scope
- Responsive dark dashboard shell.
- Fixtures date selector and refresh.
- Live centre derived from returned fixtures.
- Backend status and cache response-header display.
- Standings, analysis and predictions sections are placeholders until the exact Worker routes and response schemas are confirmed.

## Important
No API key is included in this frontend. Keep the Football API key in Cloudflare Worker secrets, never in browser JavaScript.
