# FitSystem v3.0 — Personalized Fitness PWA

A modern Progressive Web App with bottom-tab navigation, modal sheets, and personalized workout/nutrition plans for Ajeeb and Nafisha.

## What's New in v3

- **Bottom tab navigation** (Home, Workouts, Nutrition, Profile)
- **Today's workout card** auto-detects the current day
- **Week progress grid** with quick day switching
- **Modal sheets** for exercise and recipe details (industry standard)
- **Diet toggle** (Nepali/Western) on nutrition tab
- **Profile pages** with macro breakdowns and stats

## File Structure

- `index.html` — Profile selection landing page
- `ajeeb.html` — Ajeeb's plan (Push/Pull/Legs, lean bulk)
- `nafisha.html` — Nafisha's plan (Tone & Sculpt, fat loss)
- `manifest.json` — PWA manifest
- `sw.js` — Service worker (cache version: v5)
- `icon-192.png`, `icon-512.png` — App icons

## Deployment

1. Upload all files to GitHub repo
2. Settings -> Pages -> Deploy from main branch / root
3. Wait 1-2 min
4. Visit `https://USERNAME.github.io/REPO-NAME/`

## Forcing Updates

The service worker caches everything. To push an update:
1. Open `sw.js`
2. Change `const CACHE = 'fitsystem-v5';` to `'fitsystem-v6'`
3. Commit and push

Users will get the new version on next app open.

## Installing as App

**iPhone Safari:** Share -> Add to Home Screen -> Add  
**Android Chrome:** Menu -> Install App / Add to Home Screen
