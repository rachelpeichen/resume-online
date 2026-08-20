# CLAUDE.md

Personal resume site — vanilla HTML/CSS in `index.html`, deployed on Cloudflare Workers.
Live: https://resume-online.rachel-hp-chen.workers.dev/

## Workflow (required)

1. **Always branch off `main` before making changes.** Never commit directly to `main`.
   Create a fresh feature branch from `main` at the start of any new work
   (e.g. `feat/justify-text`, `fix/contact-rwd`).
2. Make the changes and commit them on that feature branch.
3. **When the work is done, ask Rachel whether to deploy before pushing/merging.**
   Do NOT auto-deploy — she wants to conserve deploy/build traffic. Wait for her
   go-ahead before pushing to `main` or triggering a Cloudflare deploy.

Rationale: pushing to `main` can trigger a Cloudflare Workers build/deploy, so
changes are batched onto a branch and deployed only on explicit request.
