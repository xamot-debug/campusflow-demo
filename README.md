# CampusFlow v2.2 — GitHub-only demo

This package is a self-contained static website for GitHub Pages.

## Supabase status

This build is intentionally disconnected from Supabase. It does not load the Supabase JavaScript client, read a project URL or publishable key, authenticate remotely, read shared cloud state, or write to remote tables. On first load it removes the prior CampusFlow Supabase browser configuration and cached Supabase Auth token keys, while preserving `campusflow-demo` browser data.

The existing Supabase project and its database/auth users are not deleted or changed by this package. They remain separate and untouched.

## Demo access

- Administrator: `ADMIN101`
- Coordinator: `CDNT101`
- Faculty: `FAC01`–`FAC08`
- Student Groups: `GRP01`–`GRP04`
- Demo password: `123456`

## Data behaviour

CampusFlow stores demo changes in browser `localStorage` under `campusflow-demo`. Each browser profile/device has its own copy. Changes do not sync between users or devices. Email notifications are previews only; no email is sent.

## GitHub Pages deployment

1. Create a GitHub repository.
2. Upload the contents of this folder to the repository root (especially `index.html` and `.nojekyll`).
3. In repository Settings → Pages, select deployment from the `main` branch and `/ (root)`.
4. Save and wait for GitHub Pages to publish the site.

No build step, package installation, environment variables, or API keys are required.
