# Watch Rate Log

A phone web app for watchmakers. Photograph a watch dial once a day, tap the hands on the photo, and the app works out how many seconds the watch gains or loses per day and over a week.

## How it works

1. Add a watch. Wind it and keep it running; it doesn't need to show the right time.
2. Once a day, tap **Photograph watch** and take a sharp, square-on photo with the seconds hand visible.
3. **In the claude.ai version, AI reads the hands for you.** It places the centre, 12 o'clock, minute-hand and seconds-hand points and names the watch it sees. Check the lines sit on the hands and save. If one is off, tap that step and place it yourself.
   In the GitHub Pages version (no AI), tap the points yourself: the centre of the hands, the 12 o'clock marker, the tip of the minute hand, and the tip of the seconds hand. There is a magnifier for accuracy. Small-seconds sub-dials are supported.
4. **The first photo is the starting point and counts as 0 s.** From the second photo on, the app shows the seconds (or minutes and seconds) gained or lost since that first photo, timed against the phone's clock. It shows:
   - the average rate in **seconds per day** (a best-fit line through all readings),
   - the expected gain or loss **per 7 days**,
   - the total gained or lost since the first photo, and whether the rate is within chronometer limits (−4 / +6 s/day).

Keep **Automatic date and time** turned on in the phone settings, so the reference clock is network-synced.

## Installing it on a Samsung phone

The app is published with GitHub Pages at **https://chappers334.github.io/README/**

1. Open that address in **Chrome** or **Samsung Internet** on the phone.
2. Chrome: menu (⋮) → **Add to Home screen** → **Install**. Samsung Internet: menu (☰) → **Add page to** → **Home screen**.
3. It opens full-screen from its own icon, like a normal app, and works offline.

Readings and photos are stored on the phone. Uninstalling the app or clearing the browser's site data deletes them.

### One-time GitHub Pages setup

1. On GitHub, open the repository → **Settings** → **Pages**.
2. Under **Build and deployment**, set **Source** to **Deploy from a branch**, pick the branch that holds `index.html` and the folder **/ (root)**, then **Save**.
3. After a minute or two the address above starts working.

GitHub Pages for a private repository needs a paid GitHub plan. On a free account, make the repository public first (Settings → General → Danger Zone → Change visibility).
