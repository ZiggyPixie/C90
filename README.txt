C90 PERFORMANCE: OFFLINE IPAD APP
=================================

This folder is a complete web app that works with no connection once it has
been added to an iPad's Home Screen. It has to be hosted on a website first
(free), opened once in Safari, then added to the Home Screen.

Files (keep them together in one folder):
  index.html             the calculator
  sw.js                  saves the app on the iPad for offline use
  manifest.webmanifest   app name and icon for the Home Screen
  icon-192.png, icon-512.png, apple-touch-icon.png   icons


STEP 1. PUT THE FOLDER ON A FREE HOST (pick one)

Option A: GitHub Pages
  1. Sign in at github.com (free account) and create a new repository,
     e.g. "c90-perf". Set it to Public.
  2. Click "Add file" > "Upload files" and drag in all the files from this
     folder (not the folder itself). Click "Commit changes".
  3. Go to Settings > Pages. Under "Build and deployment", choose
     "Deploy from a branch", branch "main", folder "/ (root)". Save.
  4. After a minute the page shows your address, like
     https://YOURNAME.github.io/c90-perf/

Option B: Netlify
  1. Sign in at app.netlify.com (free account).
  2. Go to Sites > "Add new site" > "Deploy manually" and drag this whole
     folder onto the page.
  3. Netlify gives you an address like https://something.netlify.app/

Either way the address is public: anyone who has it can open the page.


STEP 2. INSTALL ON THE IPAD

  1. With a connection, open the address in Safari.
  2. Wait until the header shows "Saved for offline use".
  3. Tap the Share button, then "Add to Home Screen", then "Add".
  4. Open it from the Home Screen icon. Turn on Airplane Mode and open it
     again to confirm it works offline.

Your last inputs are remembered on the iPad.


UPDATING LATER

If the app is changed, upload the new files to the same place. In sw.js,
change the line  const VERSION = 'c90perf-v1';  to v2, v3 and so on so the
iPad knows to fetch the new copy. Then open the app once with a connection;
the update applies the next time it is opened.


Planning aid built from digitized charts in AFMS C90-135A-1900 Rev D,
Section V. It does not replace the AFM, the Beechcraft POH or the Blackhawk
supplement.
