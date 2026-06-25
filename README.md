# Sports OSINT Prediction Engine - Public Command Center

This is the public-safe static website package for the project.

It is intentionally separate from the working local engine.

## Safe To Publish

This folder contains:

- `index.html`
- `assets/security-controls.png`
- `security-controls.png`
- this `README.md`
- `DEPLOYMENT_SECURITY_RECORD.md`

It does not include:

- prediction scripts
- raw command center workbooks
- immutable receipts
- local logs
- training outputs
- model internals
- private automation files

## Daily Export Concept

The 10 AM ET pipeline can publish sanitized public dashboard artifacts:

- sport availability
- full sanitized daily command-center tables
- public hashes
- static HTML/JSON/images

The local engine, raw receipts, private command-center workbooks, logs, scripts, and model internals stay on the laptop.

## Deployment Target

Use this folder as the root of a GitHub Pages, Netlify, or Vercel static site.

Suggested GitHub repository name:

`sports-osint-prediction-engine`

Suggested live URL:

`https://<github-username>.github.io/sports-osint-prediction-engine/`
