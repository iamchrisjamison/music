# Chris Jamison Website — GitHub + Netlify Deploy

## What's in this folder
- `index.html` — the full static site (plain HTML/CSS, no build step needed)
- `assets/` — hero photo and logo images used by the page

## Deploy steps
1. Create a new GitHub repository (e.g. `chris-jamison-site`).
2. Upload `index.html` and the `assets/` folder to the repo root (drag-and-drop on github.com works, or `git add`/`commit`/`push` if using the command line).
3. Go to netlify.com → **Add new site** → **Import an existing project** → connect your GitHub account → pick this repo.
4. Leave build settings blank (no build command, publish directory = `/`, since this is plain HTML).
5. Click Deploy — Netlify gives you a live `*.netlify.app` URL immediately.
6. To use iamchrisjamison.com: in Netlify go to **Domain settings** → **Add custom domain**, then update your domain's DNS (at your registrar) to point to Netlify per their instructions.

After this, any time you push a change to the GitHub repo, Netlify automatically redeploys the live site.

## Notes
- The Shows section uses the Bandsintown widget — it will pull live tour dates automatically once the site is on a real domain.
- The Videos section embeds a YouTube video by ID — swap the `src` in the `iframe` to change it.
- Social links (Instagram/YouTube/Facebook) and contact email are already live.
