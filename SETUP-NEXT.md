# Horo Command Centre deployment

The public repository contains only the application shell. Private Horo data remains in Microsoft storage.

After GitHub Pages is live:
1. Create a Microsoft Entra **Single-page application** registration.
2. Use the exact GitHub Pages URL as the SPA redirect URI.
3. Add delegated Microsoft Graph permissions: `User.Read`, `Mail.Read`, `Files.ReadWrite`.
4. Paste the Application (client) ID into the Horo Command Centre Settings screen.
5. Sign in with the authorised Horo Microsoft account and run **Sync now**.

Private data path:
`/Horo Command Centre/Data/horo-data.json`

Do not commit client data, tender figures, API keys or Microsoft tokens to GitHub.
