# One Flow Operating Playbook (Mintlify)

This repository powers Flow’s public-facing operating manual via Mintlify.

## Quick start
1. Push this repo to GitHub.
2. In Mintlify, create a new project and connect this repo.
3. Set your custom domain (e.g., `playbook.oneflow.com`) in Mintlify → Settings.
4. Add a CNAME record in your DNS pointing `playbook.oneflow.com` to Mintlify’s target.
5. Open PRs for changes. Merge to `main` (or `release`) to deploy.

## Branch strategy (recommended)
- `develop` – drafts/WIP (internal)
- `release` – approved SOPs (site deploys from this branch)

## Structure
- `pages/` – content in MDX
- `public/` – static assets (logo, favicon)
- `mint.json` – site configuration & sidebar

## Authoring tips
- Keep tables and checklists in Markdown for clarity.
- Use <Callout>, <Steps>, <Tabs> components where helpful.
- Cross-link related SOPs for smooth navigation.