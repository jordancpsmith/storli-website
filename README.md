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

## App icon update — November 2026
The actual Storli app icon has been cropped from the supplied iPhone launch screenshot and used for:
- Header logo on the home, support and privacy pages
- Browser favicon (`favicon.png`)
- iOS Home Screen icon (`apple-touch-icon.png`)

The source crop is approximately 183 × 183 pixels and has been resized for web use. Replace the assets with the original Xcode icon export when convenient for higher resolution.

## Updating your existing live website from iPhone
In GitHub, upload the changed `index.html`, `support.html`, `privacy.html`, `styles.css`, the new `favicon.png` and `apple-touch-icon.png` to the repository root. Also upload `storli-icon.png` **inside an `assets` folder** at the root. GitHub may require the desktop site or a computer to preserve the folder path. Once committed to `main`, Cloudflare Pages automatically redeploys.
