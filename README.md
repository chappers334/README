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

## Running it on a Samsung phone

`index.html` is a single self-contained file. Host it anywhere that serves HTTPS (for example GitHub Pages: Settings → Pages → deploy from this branch), open it in Chrome or Samsung Internet, and use **Add to Home screen**. Readings and photos are stored on the phone in browser storage.
