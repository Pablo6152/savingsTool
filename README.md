Updated Budget Helper — UI + fixes + deploy workflow
==================================================

Files included:
- index.html
- style.css
- script.min.js
- .github/workflows/deploy.yml
- README.md

What I changed:
- Fixed sidebar navigation by using event delegation (navList click handler) so clicking a nav item always switches sections.
- Applied theme consistently to both #app and document.documentElement and updated <meta name="theme-color"> when theme changes.
- Added an iOS-style toggle switch in the drawer for quick theme toggle.
- Strengthened glass UI and dark-theme contrasts; ensured most elements use CSS variables so themeing is consistent.
- Created a minified script (script.min.js) referenced by index.html for faster loads.
- Added GitHub Actions workflow to deploy to Cloudflare Pages (requires secrets: CLOUDFLARE_API_TOKEN and CLOUDFLARE_ACCOUNT_ID).

How to use:
1. Replace these files in your repo root (or docs/ if you host from docs).
2. Commit & push to main branch.
3. Add repository secrets: CLOUDFLARE_API_TOKEN and CLOUDFLARE_ACCOUNT_ID (and ensure the token has Pages write permission).
4. GitHub Actions will run and call wrangler to deploy assets.

Git commands (example):
  git checkout -b ui-refine
  git add index.html style.css script.min.js .github/workflows/deploy.yml README.md
  git commit -m "UI refine + nav fix + deploy workflow"
  git push origin ui-refine
  # open a PR and merge to main, or push directly to main if you prefer
