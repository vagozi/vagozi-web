# vagozi.com

Simple static "Coming Soon" site for Vagozi, a subsidiary of Rally Inc.

## Deploy to GitHub Pages

1. Create a GitHub repo and push these files (`index.html`, `style.css`, `CNAME`) to the `main` branch.
2. Repo **Settings → Pages** → Source: *Deploy from a branch* → `main` / `(root)`.
3. At your domain registrar, add DNS records for `vagozi.com`:
   - `A` records for `@`:
     - `185.199.108.153`
     - `185.199.109.153`
     - `185.199.110.153`
     - `185.199.111.153`
   - `CNAME` record for `www` → `<your-github-username>.github.io`
4. In **Settings → Pages**, set Custom domain to `vagozi.com`. Once the certificate is issued, tick **Enforce HTTPS**.
5. Confirm https://vagozi.com loads with a valid SSL padlock, then reply to Twilio that the site is live.

> Note: GitHub Pages issues an SSL certificate for `vagozi.com`, and the page explicitly states
> Vagozi is a subsidiary of Rally Inc. — this is what links the business name to the website for Twilio.
> Make sure the Twilio Business Profile website URL is `https://vagozi.com`.
