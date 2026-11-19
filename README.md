# Watch Rate Log

A phone web app for watchmakers. Photograph a watch dial once a day, tap the hands on the photo, and the app works out how many seconds the watch gains or loses per day and over a week.

## How it works

1. Tap **Photograph watch**. For a new watch, the AI recognises the brand and model from the photo and then asks for the job number (both can be edited). Wind the watch and keep it running; it doesn't need to show the right time.
2. Once a day, tap **Photograph watch** and take a sharp, square-on photo with the seconds hand visible.
3. **In the claude.ai version, AI reads the hands for you.** It places the centre, 12 o'clock, minute-hand and seconds-hand points and names the watch it sees. Check the lines sit on the hands and save. If one is off, tap that step and place it yourself.
   In the GitHub Pages version (no AI), tap the points yourself: the centre of the hands, the 12 o'clock marker, the tip of the minute hand, and the tip of the seconds hand. There is a magnifier for accuracy. Small-seconds sub-dials are supported.
4. **The first photo is the starting point and counts as 0 s.** Nothing is shown until a photo is taken at least a day later (23 hours, so a daily photo taken a little early still counts). From then on, the app shows the seconds (or minutes and seconds) gained or lost since that first photo, timed against the phone's clock. It shows:
   - each day's gain or loss since the previous photo, with the running total, in the **Daily readings** list,
   - the **average gain or loss per day** (total since the first photo ÷ days), at the bottom of the list and as the headline figure,
   - the expected gain or loss **per 7 days**,
   - the total gained or lost since the first photo, and whether the rate is within chronometer limits (−4 / +6 s/day).

**Print A4** and **Print receipt** make a PDF for the current test. The receipt is sized for 80 mm receipt printers (no photos). The A4 report has a photo and the gain or loss for every day, the running total, an explanation of how the readings were captured, and the overall average daily and weekly gain or loss. Open the PDF on the phone to print or share it.

**Photos are kept exactly as taken.** The camera's own file is saved byte for byte, with no enhancement, blurring or background changes; a smaller copy is used only behind the scenes for reading the hands.

**Jobs.** Several jobs can run at once. The **Job** dropdown lists every job as job number then brand and model, current jobs first and past jobs after; choose one to see its history. *Watch options → Mark job complete* moves a job to the past jobs, and *Reopen job* brings it back. The upload button adds a photo from the gallery, using the time stored in the photo.

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
