# luiza.dev

Personal site built with Hugo and the [Digio theme](https://github.com/danapixels/digio-theme), whose layout, assets, and static files are included directly in this repository. The theme author is credited in the site footer. The theme's GPL-3.0 license is preserved in [DIGIO-LICENSE](DIGIO-LICENSE).

## Run locally

Install Hugo Extended 0.146.0 or newer, then from this directory run:

```powershell
hugo server
```

Open <http://localhost:1313/>.

## Publish

The workflow at `.github/workflows/hugo.yml` builds the site and deploys it to GitHub Pages after each push to `main`. In the repository's GitHub settings, set **Settings → Pages → Build and deployment → Source** to **GitHub Actions**. The workflow publishes to the custom domain configured in `static/CNAME` (`www.luiza.dev`).

After committing and pushing changes to `main`, check the repository's **Actions** tab for the “Deploy Hugo site to Pages” run. Once it completes, the new version is live at <https://www.luiza.dev/>.