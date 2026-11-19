# Watch Rate Log

A phone web app for watchmakers. Photograph a watch dial once a day, tap the hands on the photo, and the app works out how many seconds the watch gains or loses per day and over a week.

## How it works

1. Add a watch and set it roughly to the right time (within a few minutes).
2. Once a day, tap **Photograph watch** and take a sharp, square-on photo with the seconds hand visible.
3. On the photo, tap: the centre of the hands, the 12 o'clock marker, the tip of the minute hand, and the tip of the seconds hand. There is a magnifier for accuracy. Small-seconds sub-dials are supported.
4. The app compares the watch reading with the phone's clock at the moment the photo was taken. It shows:
   - the average rate in **seconds per day** (a best-fit line through all readings),
   - the expected gain or loss **per 7 days**,
   - the total measured change, and whether the rate is within chronometer limits (−4 / +6 s/day).

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
