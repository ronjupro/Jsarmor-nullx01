# JSArmor Website — Ronjumoz

## Deploy to Vercel (no build command needed)

1. Extract the ZIP file.
2. Open `index.html` and find `RONJUMOZ_TELEGRAM_URL` near the bottom.
3. Replace `https://t.me/ronjumodz` with your real Telegram channel invite/public URL, for example `https://t.me/your_channel`.
4. Keep the folder structure unchanged:
   - `index.html`
   - `vercel.json`
   - `assets/JSArmor.js`
5. In Vercel, choose **Add New → Project** and import the Git repository containing these files. If using the Vercel CLI, run `vercel` from this project folder.
6. Use the framework preset **Other**. No build command or output directory is required for this static site; the project root should contain `index.html`.
7. Deploy. Test the live site on mobile and desktop.

## Git-based deployment

Create a GitHub repository, upload the contents of this folder (not the ZIP itself), then import that repository into Vercel. Future commits will trigger redeployments.

## Features

- Responsive JSArmor JavaScript obfuscation UI.
- Local `.js` file input and copy output.
- Protected code downloads as `ronjumodz.js`.
- Telegram join popup shown when the site opens.
- Owner: Ronjumodz.
- Optional domain-lock field, using the included JSArmor library.

## Important setup notes

- The Telegram join popup is configured for `https://t.me/ronjumodz`.
- JSArmor's obfuscator dependency is loaded from jsDelivr, so visitors need internet access.
- This is a static website; the code is processed in the visitor's browser. Do not put secrets or API keys in frontend code.
- Obfuscation is not encryption, and domain locking is not a substitute for server-side access control.
