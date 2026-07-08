# Pocket Elite LLC — Website

Official website for [Pocket Elite LLC](https://pocketelite.store) and the **SlapPocket** iOS app.

## Pages

| Page | URL | Purpose |
|------|-----|---------|
| Homepage | `/` | Animated landing page |
| Contact | `/contact.html` | Support & inquiries |
| Privacy Policy | `/privacy.html` | Required for App Store |
| Terms of Service | `/terms.html` | App Store compliance |

## GitHub Pages Deployment

1. **Push this repo to GitHub**
   ```bash
   git init
   git add .
   git commit -m "Initial Pocket Elite website"
   git branch -M main
   git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPO.git
   git push -u origin main
   ```

2. **Enable GitHub Pages**
   - Go to your repo → **Settings** → **Pages**
   - Under **Source**, select **Deploy from a branch**
   - Choose branch: `main`, folder: `/ (root)`
   - Click **Save**

3. **Configure custom domain**
   - In Pages settings, enter `pocketelite.store` in **Custom domain**
   - The `CNAME` file in this repo is already set to `pocketelite.store`
   - At your domain registrar, add DNS records:
     - **A records** pointing to GitHub Pages IPs:
       ```
       185.199.108.153
       185.199.109.153
       185.199.110.153
       185.199.111.153
       ```
     - Or a **CNAME record**: `www` → `YOUR_USERNAME.github.io`
   - Enable **Enforce HTTPS** in GitHub Pages settings (may take up to 24 hours)

## App Store Connect URLs

When submitting SlapPocket, use these URLs:

- **Privacy Policy URL:** `https://pocketelite.store/privacy.html`
- **Terms of Service URL:** `https://pocketelite.store/terms.html` (link in App or Support URL)
- **Support URL:** `https://pocketelite.store/contact.html`
- **Marketing URL:** `https://pocketelite.store`

Also link to the Privacy Policy from within the SlapPocket app (Settings or About screen).

## Email Setup

The site references these addresses — set them up at your domain provider:

- `support@pocketelite.store` — general support
- `privacy@pocketelite.store` — privacy/data requests

## Local Preview

Open `index.html` in a browser, or run a local server:

```bash
python3 -m http.server 8080
```

Then visit `http://localhost:8080`

## License

© 2026 Pocket Elite LLC. All rights reserved.
