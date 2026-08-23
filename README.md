# ListingLeak site — GitHub Pages ($0)

Brand: ListingLeak · Toronto, Ontario  
Checkout (exact URL, no wrappers): https://listingleak.gumroad.com/l/dgzma

This folder is the full static site (home, HVAC/plumber/roofer SEO pages, privacy, CSS, sitemap, robots). Do not add trackers, fake reviews, or a different checkout URL.

## Human step required (GitHub CLI is not logged in)

On this computer, nothing is authenticated for GitHub, Surge, Netlify, Wrangler, or Vercel. Do not scrape credentials. Do not spend money.

1. In a terminal here, run:

   ```bash
   gh auth login
   ```

   Use GitHub.com, HTTPS, and an account you control.

2. Publish Pages from this folder:

   ```bash
   cd /workspace/listingleak/site
   git init
   git add .
   git commit -m "ListingLeak public site"
   gh repo create listingleak --public --source=. --remote=origin --push
   gh api -X POST repos/$(gh api user --jq .login)/listingleak/pages \
     -f "source[branch]=main" -f "source[path]=/"
   ```

3. Live URL after Pages builds (usually a few minutes):

   `https://<github-username>.github.io/listingleak/`

   Confirm `gh api user --jq .login` after login; do not guess a username.

## Do not

- Buy a custom domain or paid plan.
- Wrap the Gumroad URL in a redirector.
- Put a personal legal name, Stratford, or a home address/phone on this site.
- If a form requires a person name, use **Tom** only.

## NAP

- Name: ListingLeak
- Area: Toronto, Ontario
- No street address (none is public; do not invent one)
- Payment: Gumroad checkout above
