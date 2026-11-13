TRAINING LOG v0.3

INSTALL / UPDATE
1. Unzip this package.
2. Upload index.html, manifest.webmanifest and sw.js to the root of your existing GitHub Pages repository.
3. Commit the changes and wait for GitHub Pages to deploy.
4. Re-open the same site on your iPhone. If the old version remains, close the PWA and reload the site in Safari.

IMPORTANT DATA NOTE
This update keeps the existing localStorage key (training-log-v1) and migrates your current data in place. Export a JSON backup from Settings before updating anyway. Your workouts are stored locally in the browser on this device and are not synced to a server.

WHAT'S NEW
- Editable workout templates with exercise order, target sets and rep ranges.
- Workout elapsed timer; saved gym duration.
- Run and hockey duration entry plus an in-form stopwatch.
- Weekly active time totals across gym, running and hockey.
- Clickable activity history with gym workout breakdowns and run/hockey details.
- Per-set previous-session values and all-time heaviest logged set remain visible while training.
- Import a Garmin GPX export into a run to display its GPS track.

GARMIN LIMITATION
Automatic Garmin Connect syncing is not implemented in this static GitHub Pages build. Secure automatic syncing needs an authenticated backend and must not expose Garmin credentials in browser code. GPX route import is the interim option. The route display is a trace, not a street-map basemap. Garmin FIT metrics such as heart rate, cadence, elevation and pace splits are not parsed in this version.

BACKUP
Use Settings > Export backup regularly. Keep the JSON file somewhere safe.
