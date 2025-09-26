
# IAPT Website — iaptus.org

A clean, bilingual (EN/中文) static site for the Institute for Applied Process Thought (IAPT).

## Quick Deploy: GitHub Pages

1. Create a new GitHub repo (e.g. `iaptus-site`) and upload all files.
2. In **Settings → Pages**, set **Build from**: `Deploy from a branch`, select `main` and `/root`.
3. Commit the included `CNAME` file that contains `iaptus.org`.
4. In your domain DNS:
   - Set `www` as a **CNAME** to `<your-github-username>.github.io`.
   - For the apex/root `iaptus.org`, either:
     - Use your DNS provider's **ALIAS/ANAME** to the same target, or
     - Use **A** records per GitHub Docs (IP addresses can change; always check latest official docs).
5. Wait for DNS to propagate. In Pages settings, enable **HTTPS** when available.

Docs:
- GitHub Pages custom domains & apex configuration (official docs)
- HTTPS certificates via Let's Encrypt (auto)
- Domain verification (optional but recommended)

## Alternative: Netlify (free)

1. Drag & drop this folder into Netlify or connect the GitHub repo.
2. Add your custom domain `iaptus.org` in **Domain management**.
3. Follow Netlify’s prompts to set DNS (either Netlify DNS or External DNS).

## Customize

- Edit content in `index.html`, `about.html`, etc.
- Styles live in `css/styles.css`.
- Replace `img/logo.svg` with your logo if you have one.

## Notes
- Keep `404.html` for better routing.
- If you later add blogs or more pages, consider a static site generator (Jekyll/Hugo/Eleventy).
