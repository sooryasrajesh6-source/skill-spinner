🎡 Skill Spinner

Can't decide what to practice? Spin the wheel.

Skill Spinner is a free, offline-capable web app that helps you build skills through daily practice. Add the skills you want to learn, spin the wheel to pick one, set a practice plan, and keep your streak going.

Open the app · works on phone and desktop · no sign-up · no ads

<!-- Add screenshots here, e.g. ![Spin screen](screenshots/spin.png) ![Today screen](screenshots/today.png) ![History screen](screenshots/history.png) -->
How it works
Add your skills. Guitar, Spanish, drawing, coding, anything you want to get better at.
Spin the wheel. It picks the skill to focus on for the next week or more.
Set your plan. Choose the challenge length (1 to 4 weeks) and minutes per day.
Practice and check in daily. Build a streak and fill in the day-by-day grid.
Review your progress. The History tab shows days practiced, estimated minutes and completion for each skill.
Features
Animated spin wheel with your own skills
Daily check-in with streak counter
Configurable challenge duration and daily time
Per-skill progress and history
Installable as an app (PWA) on Android, iPhone and desktop
Works offline after the first visit
Light and dark mode follow your device setting
All data stays on your device (localStorage), nothing is sent anywhere
Install on your phone
Android (Chrome): open the link, then menu → Install app.
iPhone (Safari): open the link, then Share → Add to Home Screen.
Run locally
bash
git clone https://github.com/YOUR-USERNAME/skill-spinner.git
cd skill-spinner
python3 -m http.server 8000

Then open http://localhost:8000. (Service workers need localhost or HTTPS, so opening the file directly won't enable offline mode.)

Project structure
index.html      the whole app (HTML, CSS and JavaScript)
manifest.json   PWA name, colors and icons
sw.js           service worker for offline support
icons/          app icons

When you change index.html, bump the cache name in sw.js (skill-spinner-v1 → v2) so returning users get the update.

Limitations
Data is stored per device and browser. There is no cloud sync, so clearing browser data erases your progress.
Only one challenge can be active at a time.
Roadmap ideas
Export/import data for backup
Daily reminder notifications
Grace day for missed streaks
Self-rating to measure progress
Optional accounts and sync
Contributing

Issues and pull requests are welcome. Open an issue first for larger changes.

License

MIT, see LICENSE.
