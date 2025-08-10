Budget Helper - production-ready static site
------------------------------------------
Files:
- index.html
- style.css
- script.js
- wrangler.jsonc

Deploy with Cloudflare Pages (wrangler):
1. unzip/clone this folder and cd into it
2. run: npx wrangler deploy
   or explicitly: npx wrangler deploy --assets=.
3. After deploy you'll get a Pages URL to open in Safari on your iPhone.

Notes:
- No dummy data included. All data stored in browser LocalStorage.
- Use Export JSON in Settings to back up data.
