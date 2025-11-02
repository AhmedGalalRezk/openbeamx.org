# Deploy to GitHub Pages (Free)

1. **Create a GitHub repo** named `openbeamx.github.io` (or any name).
2. Upload all files from this folder to the repo root.
3. In the repo, go to **Settings → Pages** and set Source to **Deploy from a branch**, select `main` and `/ (root)`.
4. Add the custom domain:
   - In **Settings → Pages** set **Custom domain** to `openbeam.org`.
   - Ensure the file `CNAME` exists in repo root containing exactly: `openbeam.org`.
5. In your domain registrar (where you buy the domain), add **DNS records**:
   - `A` records pointing to GitHub Pages IPs:
     - 185.199.108.153
     - 185.199.109.153
     - 185.199.110.153
     - 185.199.111.153
   - Optional: `AAAA` records for IPv6 (see GitHub Pages docs).
6. Wait for DNS to propagate (usually 15–60 minutes). Visit `https://openbeam.org`.

**Note:** You can also deploy free via Netlify or Cloudflare Pages. Upload this folder, set `index.html` as the entry, and add your custom domain in their dashboard.
