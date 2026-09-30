# Horo Command Centre V4

Phone-first Horo Constructions operations dashboard.

## Security model
The GitHub repository contains only the application shell. It does **not** contain client names, job addresses, job costs, tender figures, Outlook messages, SharePoint file contents or API keys.

Private Horo data is loaded in the user's browser after Microsoft sign-in from:
`/Horo Command Centre/Data/horo-data.json`

Microsoft tokens are kept in browser `sessionStorage`. The QLDTraffic key, if supplied, is stored only in the local browser and must never be committed to GitHub.

## Deployment
GitHub Pages workflow is included at `.github/workflows/pages.yml`.

## Microsoft setup
After the first Pages deployment, create a Microsoft Entra SPA app registration and add the final GitHub Pages URL as the SPA redirect URI. Delegated permissions used by V4 are:
- User.Read
- Mail.Read
- Files.ReadWrite

Paste the Application (client) ID into Settings in the app.
