Render deployment steps
=======================

1. Create a GitHub repo and push the `portfolio` folder as the repository root.

   Example commands (run from the `portfolio` directory):

   ```powershell
   git remote add origin git@github.com:YOUR_USERNAME/YOUR_REPO.git
   git push -u origin main
   ```

2. On Render (https://render.com), create a new service -> Static Site.
   - Connect your GitHub account and select the repo.
   - Branch: `main`
   - Build command: leave blank
   - Publish directory: `.`
   - Create service.

3. After deployment, Render will provide a permanent URL and you can add a custom domain if desired.

Notes:
- If you prefer, use GitHub Pages, Vercel, or Netlify instead — those are free and simple for static sites.
- Replace `REPLACE_WITH_GITHUB_REPO_URL` in `render.yaml` with your repo URL if you want the config fully filled.
