# Voicecart Project Rules

## Deployment Workflow
1. **Always work on `dev` branch** - All changes go to the `dev` branch during work sessions
2. **Push to dev frequently** - Commit and push to `dev` after completing changes
3. **Ask before deploying to production** - At the end of each session or after major changes, ask: "Should I merge to main and deploy to Netlify?"
4. **Only merge to `main` when approved** - Merging to `main` triggers Netlify auto-deploy, so only do this when the user confirms

## Branch Structure
- `dev` - Working branch for ongoing changes (does NOT trigger Netlify deploy)
- `main` - Production branch (auto-deploys to Netlify)

## Project Overview
**VoiceCart** - A landing page selling Apple Shortcuts that let iPhone users voice-search Instacart stores.

### Key Files
- `index.html` - The entire landing page (single-page site)
- `demo.mp4` - Hero section video showing the shortcut in action (plays in iPhone mockup)

### Site Structure (in index.html)
- **Hero section** - iPhone mockup with auto-playing demo video
- **Scrolling store ribbon** - Animated horizontal scroll of store pills
- **How It Works** - 3-step explanation
- **Use Cases** - Who it's for (busy parents, professionals, etc.)
- **Stores section** - All 27+ supported stores as clickable pills
- **Pricing section** - $10 all stores bundle OR $3 single store with search/selector
- **FAQ section** - Collapsible Q&A
- **CTA + Footer**

### Key Features Built
- Store pills (both sections) are clickable → scroll to pricing & pre-select that store
- Store selector with search in pricing section
- Checkout buttons link to Polar.sh payment links
- Device warning banner shows for non-iPhone visitors (Android/desktop)
- iPhone mockup visible on mobile (smaller size)

### Tech Stack
- Tailwind CSS (via CDN)
- Vanilla JavaScript (no framework)
- Hosted on Netlify (auto-deploys from main)
- Payments via Polar.sh

### Payment Links
Store checkout links are defined in `storeCheckoutLinks` object in the inline JavaScript (~line 640)
