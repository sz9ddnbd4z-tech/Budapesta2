# HomeScout — deployment

1. Import GitHub repo `sz9ddnbd4z-tech/Budapesta2` in Vercel, select branch `homescout-pawson-preview` and framework `Other`.
2. Set server environment variables `NOTION_TOKEN` (Notion integration secret with access to the apartment database) and `HOMESCOUT_ACCESS_KEY` (strong independent access key).
3. Enable Vercel Deployment Protection / authentication. Do not publicly expose the property collection or its edit endpoint.
4. Deploy. Visit root URL, click `Połącz z Notion`, enter only the HOMESCOUT_ACCESS_KEY, not the Notion secret.
5. Confirm live GET and PATCH to Notion, including reload from another device.
6. Verify all listing URLs and images; missing photographs must remain clearly marked, never substituted with stock images.

Without steps 1–3 the frontend is a read-only snapshot and must not be represented as live synced.
