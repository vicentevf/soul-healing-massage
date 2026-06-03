# Soul Healing Massage Therapy — Website

Single-page website for [Soul Healing Massage Therapy](https://www.fresha.com/a/soul-healing-massage-therapy-mount-maunganui-632-grenada-street-cfspcm6z), Mount Maunganui, NZ.

## Stack

- Pure HTML + CSS + vanilla JS (no build step, no framework)
- Google Fonts: Fraunces + Inter Tight
- All bookings go through Fresha

## File Structure

```
.
├── index.html      # The entire site (single page, no build needed)
├── images/         # Studio photos + logo
│   ├── hero-main.jpg
│   ├── hero-sub.jpg
│   ├── about.jpg
│   └── logo.png
├── .nojekyll       # Disables Jekyll processing on GitHub Pages
└── .gitignore
```

## Before going live

⚠ **The WhatsApp button has a placeholder phone number.**

In `index.html`, search for `64XXXXXXXXX` and replace with Kati's WhatsApp number in international format (country code + number, no spaces or symbols).

Example for a New Zealand mobile `021 123 4567` → `64211234567`.

## Local preview

Just open `index.html` in any browser — no server needed.

For a quick local server (optional):
```bash
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Deploy to GitHub Pages

1. Push this folder to a new public GitHub repo
2. Go to **Settings → Pages**
3. Source: **Deploy from a branch**, Branch: **main**, Folder: **/ (root)**
4. Save. After ~1 minute the site will be live at `https://YOUR_USERNAME.github.io/REPO_NAME/`

To use a custom domain (e.g. `soulhealingmassage.co.nz`):
1. Add a `CNAME` file containing just the domain name
2. In your domain registrar's DNS, add a CNAME record pointing to `YOUR_USERNAME.github.io`
3. In GitHub **Settings → Pages**, enter the custom domain and enable HTTPS

## Updating content

Just edit `index.html` (it's a single file with everything) and push to the `main` branch. GitHub Pages will redeploy automatically within a minute.
