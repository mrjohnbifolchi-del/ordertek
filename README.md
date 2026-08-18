# Ordertek.ca – Static Website

Clean, professional static site for Ordertek forensic workstations.

## Structure
- `index.html` – Home
- `workstations.html` – Example configurations
- `about.html` – About the company
- `contact.html` – Quote request (email + simple form)
- `css/styles.css` – All styles
- `404.html` – Custom 404
- `robots.txt`

## Deploy to Cloudflare Pages (Free)

### Option A – Direct Upload (fastest)
1. Go to Cloudflare Dashboard → Workers & Pages → Create → Pages → Upload assets
2. Project name: `ordertek` (or whatever you like)
3. Upload the entire contents of this folder (the files inside `ordertek-site`, not the folder itself)
4. Deploy

### Option B – Git (recommended for updates)
1. Create a GitHub repo and push this folder
2. In Cloudflare Pages → Create → Connect to Git → select the repo
3. Build settings:
   - Framework preset: None
   - Build command: (leave empty)
   - Build output directory: `/` (or `.`)
4. Deploy

### Custom Domain
1. In the Pages project → Custom domains → Set up a domain
2. Add `ordertek.ca` and `www.ordertek.ca`
3. Cloudflare will guide you to update nameservers (or add the CNAME if the domain is already on Cloudflare)

### After launch
- Update the email address if `info@ordertek.ca` is not the final one
- Replace the text logo with a real logo image if desired (place in `/images/` and update the HTML)
- Optional: Connect a free form backend (Formspree, Basin, or Cloudflare Workers + Email) instead of the mailto form

## Notes
- All prices noted as CDN
- 3-year hot-swap warranty messaging retained
- Specs are cleaned-up versions of the current live examples
- Contact method simplified to direct email + lightweight form
