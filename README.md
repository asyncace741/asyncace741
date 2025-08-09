# Hi, I'm **Prabath Wanasinghe** 👋


## About this profile card
A clean, professional and customizable GitHub profile header using a **pink / dark-blue translucent** gradient.  
It shows a dynamic greeting and current date & time (kept up-to-date by a GitHub Action).

### Features
- Pink ↔ Dark Blue translucent gradient (modern & sleek)
- Real-time looking greeting: `Hello "Myname", Good morning/afternoon/evening/night`
- Current date & time (updated automatically by GitHub Action)
- Easy to customize (name, colors, fonts, layout)
- Professional, responsive SVG design — renders in README on GitHub

---

## Customize
Edit `scripts/config.json` to change:
- `name` — your display name
- `primaryColor` / `secondaryColor` — gradient colors (hex)
- `accent` — accent color used for small accents
- `timezone` — optionally set your timezone for formatting (e.g., `"Asia/Colombo"`)

## Files added to repo
- `profile-card.svg` — generated image shown in this README
- `.github/workflows/update-readme.yml` — action that regenerates the SVG on schedule
- `scripts/generate-svg.js` — Node script that generates `profile-card.svg`
- `scripts/config.json` — small config file for name/colors/timezone

---

## Quick start
1. Copy the files below into your repo.
2. Open `scripts/config.json` and set `"name"` to your name.
3. Push to GitHub — enable GitHub Actions if prompted.
4. The Action will run on schedule and update `profile-card.svg`. The README will display the latest SVG.

---

## Notes & limitations
- GitHub does not run client-side JavaScript in markdown; dynamic updates are achieved by regenerating the SVG from Actions.
- The Action runs on the schedule you choose (default every 5 minutes is shown; you can change it).
- SVG is generated server-side; it will update when Action runs and commits a new SVG.
