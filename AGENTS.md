# Project Context for Codex

## Overview

This repository contains the static personal website for Sippanon Kitimoon, Ph.D. The site presents an academic and applied data science profile for GitHub Pages.

- Repository: `git@github.com:skitimo/website.git`
- Public site: `https://skitimo.github.io/website/`
- Hosting: GitHub Pages from the `main` branch, `/ (root)` folder
- Site language: English-only for the current version
- Current audience: collaborators, hiring and consulting contacts, CMU students and faculty, and academic readers

The repository is public. Treat all committed content as publicly accessible, including the CV PDF and image assets.

## Tech Stack

This is a buildless static site.

- `index.html`: single-page website
- `assets/css/styles.css`: all styling
- `assets/images/`: visual assets
- `files/kitimoon_cv.pdf`: published CV file
- `.nojekyll`: keeps GitHub Pages from applying Jekyll processing

There is no package manager, bundler, framework, or generated build output.

## Key Content Sources

The first version was based on:

- `kitimoon_cv.pdf`
- The CMU / Faculty of Science / DSRC welcome poster
- User answers documented in `plan.md`

Important public profile details already reflected in the site:

- Name: Sippanon Kitimoon, Ph.D.
- Affiliation: Data Science Research Center, Faculty of Science, Chiang Mai University
- Focus areas: data science, signal processing, machine learning, applied mathematics, computational harmonic analysis
- Google Scholar: `https://scholar.google.com/citations?user=DyFbVikAAAAJ`
- Public email target should be kept consistent as `sippanon.kitimoon@cmu.ac.th` unless the user asks otherwise

## Important Assets

- `assets/images/sippanon-headshot.jpeg`: homepage hero headshot and Open Graph preview image
- `assets/images/welcome-poster.jpeg`: original welcome poster source
- `assets/images/kitimoon_qr.png`: QR image asset supplied later by the user
- `assets/images/favicon.svg`: simple favicon
- `files/kitimoon_cv.pdf`: downloadable CV

If replacing a public image, prefer a new filename when cache busting matters, then update both the visible `<img>` reference and the Open Graph image metadata in `index.html`.

## Local Preview

Run from the repository root:

```sh
python3 -m http.server 4173
```

Open:

```text
http://127.0.0.1:4173/
```

Quick checks:

```sh
curl -I http://127.0.0.1:4173/
curl -I http://127.0.0.1:4173/files/kitimoon_cv.pdf
```

## Deployment

Deployment is automatic after pushing to `main`.

Expected live URL:

```text
https://skitimo.github.io/website/
```

GitHub Pages is configured in GitHub settings to deploy from:

- Branch: `main`
- Folder: `/ (root)`

After pushing, check the Pages workflow and live site:

```sh
curl -sS 'https://api.github.com/repos/skitimo/website/actions/runs?per_page=1'
curl -I -L https://skitimo.github.io/website/
```

GitHub Pages may briefly serve cached content or a 404 while a deployment is still running.

## Workflow Preferences

- Use conventional commits.
- Keep changes small and scoped.
- Check `git status --short --branch` before editing, staging, committing, or pushing.
- Do not overwrite or revert user changes unless the user explicitly asks.
- Use `rg` for text search.
- Use `apply_patch` for manual file edits.
- Commit and push when the user asks for a change that needs to be available from another computer.

Recent commit examples:

- `feat: implement personal website`
- `docs: update contact email and image assets`
- `fix: update website headshot asset`

## Design Direction

The site should remain professional, clear, and academic rather than a marketing landing page.

- Keep the first screen focused on identity, expertise, CV, Scholar, and email.
- Keep layouts responsive and readable on mobile.
- Avoid clutter from the original poster; use it only as context or source material.
- Preserve the quiet, technical feel with CMU/DSRC-inspired accents.
- Use direct section names and concise text.

## Safety Notes

- The repository and GitHub Pages site are public.
- Confirm before adding phone numbers, personal addresses, private documents, unpublished manuscripts, private IDs, or other sensitive details.
- Do not type or store passwords, tokens, or private keys in the repo.
- If GitHub asks for sudo-mode password or account authentication, the user must enter it directly.

## Known Follow-Up Ideas

Potential future improvements:

- Add ORCID, GitHub, LinkedIn, CMU profile, or ResearchGate links after the user confirms exact URLs.
- Add selected publications with citations and links.
- Add course or teaching pages for CMU.
- Add a custom domain if the user provides one.
- Add cache-busted asset filenames when replacing public images.
