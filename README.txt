TRAINING LOG v0.4 - GARMIN CONNECT

UPDATE YOUR EXISTING APP
1. Export a backup in Training Log > Settings before updating.
2. Download and unzip this package.
3. Upload index.html, manifest.webmanifest and sw.js to the root of your existing GitHub Pages repository, replacing the old files.
4. Commit the changes and wait for GitHub Pages to deploy.
5. Close the installed app, open the site in Safari, reload it, then reopen the Home Screen app.

CONNECT GARMIN
1. Open Training Log > Settings.
2. Paste your Cloudflare Worker URL, e.g. https://training-log-garmin.YOUR-SUBDOMAIN.workers.dev
3. Enter the APP_ACCESS_PASSWORD you created in Cloudflare.
4. Tap Sync Garmin activities.
5. Open a Garmin run in History and tap Load GPS & detailed data.

WHAT IT DOES
- Retrieves up to 50 recent Garmin activity summaries through your existing Cloudflare Worker.
- Imports activities into local Training Log history and updates existing Garmin records without duplicating them.
- Downloads the original Garmin activity ZIP on demand.
- Unzips the FIT file in the browser and parses GPS trackpoints, heart-rate samples, cadence, altitude and lap splits.
- Displays route trace, pace, heart rate, calories, cadence, elevation and available splits on activity detail pages.

PRIVACY AND LIMITATIONS
- Your Garmin Personal API key stays in Cloudflare.
- The Cloudflare app password is entered in Training Log and held in memory for the current page session only. It is not saved in the app's localStorage or backup.
- Activity data and imported FIT-derived details are stored locally on this iPhone in the existing training-log-v1 storage.
- Sync requires an internet connection and the Cloudflare Worker already deployed in your previous setup.
- The route is shown as a GPS trace, not a street-map basemap.
- The app does not upload your local workouts to Garmin.

DATA SAFETY
This release keeps the existing localStorage key training-log-v1. Export a backup before updating. Do not clear Safari website data.
