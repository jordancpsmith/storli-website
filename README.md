# Storli website

Static site for storliapp.co.uk. Deploy via Cloudflare Pages with Git integration.

## Cloudflare Pages setup
1. Create a new GitHub repository for this website (separate from the app's source repository).
2. Upload the contents of this directory to the repository root.
3. In Cloudflare, go to Workers & Pages > Create > Pages > Connect to Git.
4. Select the repository, use a static site configuration (no build command; output directory `/`), and deploy.
5. Add `storliapp.co.uk` under the Pages project's Custom domains and follow Cloudflare's DNS prompts.
6. Confirm HTTPS, homepage, support and privacy URLs work.

## Before public launch
- Replace the illustrative feature panel with actual app screenshots.
- Verify feature and subscription descriptions against the shipping app.
- Complete and legally review the privacy policy, including marketplace integrations, data processing and retention.
- Confirm support@storliapp.co.uk can send and receive email.
- Add App Store listing URL once live.

No DNS records for iCloud Mail need to be modified to publish the website. Preserve MX, SPF, DKIM and Apple verification records.

## Branding revision (November 2026)
- Updated to the established Storli mint/teal palette: `#3ED1A6`, `#2BBF96`, `#0B2A2F`, `#F4F6F6`.
- Added responsive hero, refined inventory illustration, premium Pro section, hover/focus states and reduced-motion support.
- The small box/pin SVG in the header is **an illustrative placeholder**, not the verified original app logo. Replace it with the approved production icon when available.
- The inventory preview is explicitly illustrative, not a real screenshot.
- The privacy page remains an incomplete draft and **must not be used as the final App Store privacy policy**.
- No analytics, trackers, external fonts or third-party scripts are included.


## Updated app showcase (November 2026)
- `assets/storli-app-showcase.png` is an **illustrative recreation** based on the two provided Storli screenshots, with fictional sample entries replacing the owner's Recent Activity items and no visible iOS status bar. It is not an exact screenshot of the running app.
- The homepage includes the showcase in its hero and in a dedicated feature section.
- Upload the whole ZIP's contents to the root of the GitHub `storli-website` repository, preserving the `assets/` directory.
- Check the Privacy page before publishing as an approved legal policy.
