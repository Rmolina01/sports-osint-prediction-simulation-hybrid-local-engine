# Deployment Security Record

## Purpose

Prepare a public coming-soon website without exposing the working local Sports OSINT Prediction Engine.

## Public Package

Folder:

`showcase/Sports-OSINT-Coming-Soon/`

Files:

- `index.html`
- `README.md`
- `DEPLOYMENT_SECURITY_RECORD.md`
- `assets/security-controls.png`
- `security-controls.png`

## Security Decisions

- Publish only a static presentation site.
- Do not publish `work/`.
- Do not publish `outputs/`.
- Do not publish raw receipts, logs, command-center workbooks, or model scripts.
- Do not publish local filesystem paths in the public page.
- Publish only sanitized daily display outputs; keep raw evidence and model internals private.
- Use public language: architecture, safety, coming soon, private beta.

## Recommended Hosting

GitHub Pages, Netlify, or Vercel static hosting.

For GitHub Pages:

1. Create a repository named `sports-osint-prediction-engine`.
2. Upload only the contents of this folder.
3. Enable GitHub Pages from `main` branch and `/root`, or use the included static Pages workflow.
4. Use the Pages URL in the external showcase form.

## Daily Update Channel

For automatic 10 AM ET updates, use a repository-scoped SSH deploy key. The private key stays local; the public key is added to the GitHub Pages repository. The deploy script should push only the sanitized public export folder.

## Public Table Policy

The website may show full sanitized daily command-center tables for sharing with trusted friends or a public audience. These tables are display artifacts only. They must not contain source workbooks, raw receipts, training logs, local paths, scripts, model weights, private automation files, or credentials.

## Local Engine Boundary

The local engine remains in the main workspace and continues to run from:

`work/mlb_osint/run_daily_mlb_osint.ps1`

The public site is not part of the training, prediction, simulation, or integrity workflow.
