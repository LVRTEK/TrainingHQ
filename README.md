# TrainingHQ

A mobile-first training session planner and timer for youth basketball coaches. Companion app to RotationHQ.

## What it does
- Pick a team, set session details (date, venue, target length)
- Build a session from a drill library (or your own custom drills) organised by category
- Run the session with a live timer: drill countdown, overall court-time clock, and a delta indicator showing whether you're ahead or behind schedule
- Save completed sessions with attendance and notes, and review them later

## Deploying to GitHub Pages

1. Create a new repository on GitHub (or use an existing one), e.g. `traininghq`.
2. Upload `index.html` to the root of the repository (drag-and-drop on the GitHub web UI works fine, or push via git).
3. In the repo, go to **Settings → Pages**.
4. Under **Source**, select **Deploy from a branch**, choose the `main` branch and the `/ (root)` folder, then **Save**.
5. GitHub will give you a live URL, usually `https://<your-username>.github.io/<repo-name>/` — it can take a minute or two to go live after the first deploy.

If you want it alongside RotationHQ in the same repo, just drop `index.html` into a subfolder (e.g. `/training/index.html`) instead of the root, and it'll be available at `https://<your-username>.github.io/<repo-name>/training/`.

## A note on data storage
This version stores teams, your custom drill library, and saved session history in the browser's local storage on whichever device opens it. That means:
- Data does **not** sync between your phone and laptop, or between different browsers on the same device.
- Clearing your browser's site data (or using a different browser/incognito mode) will reset it.

This is fine for trying it out solo, but if you want it to work properly across devices or for other coaches to use without losing their data, we'd want to add a proper backend (a small database) down the track — happy to talk through options when you're ready for that step.
