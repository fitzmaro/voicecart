# Voicecart Project Rules

## Deployment Workflow
1. **Always work on `dev` branch** - All changes go to the `dev` branch during work sessions
2. **Push to dev frequently** - Commit and push to `dev` after completing changes
3. **Ask before deploying to production** - At the end of each session or after major changes, ask: "Should I merge to main and deploy to Netlify?"
4. **Only merge to `main` when approved** - Merging to `main` triggers Netlify auto-deploy, so only do this when the user confirms

## Branch Structure
- `dev` - Working branch for ongoing changes (does NOT trigger Netlify deploy)
- `main` - Production branch (auto-deploys to Netlify)

## Project Info
- Simple static HTML page (index.html)
- Hosted on Netlify (auto-deploys from main branch)
- No build process required
