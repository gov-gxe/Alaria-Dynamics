# GitHub Pages deployment for Aaria Dynamics

This repository uses GitHub Pages to host the static prototype site under the `docs/` folder.

Recommended settings (Repository > Settings > Pages):

- Source: Branch `main`
- Folder: `/docs`
- Enforce HTTPS: Enabled (recommended)

Verification steps after enabling Pages:

1. Visit the repository Settings -> Pages and confirm the source shows "main branch /docs folder".
2. Wait a minute or two for the site to build and note the published URL shown in the Settings page.
3. If assets appear unstyled, ensure files are referenced with relative paths (e.g. `assets/styles.css`), not absolute paths starting with a leading slash.
4. If you need a custom domain, add it in the Pages settings and verify DNS records per GitHub's guide.

Notes and troubleshooting:

- If the Pages build fails, check `Actions` -> `Pages` for build logs; common issues include files missing from `docs/` or incorrect paths.
- During development, you can preview the `docs/` folder locally by serving it with a simple static server (e.g., `python -m http.server 8000` from the `docs` folder).

If you'd like, I can add a small staging workflow or GitHub Actions to validate builds and run a link-checker before publishing.
