# Tally

A simple monthly budgeting app in a single HTML file. No install, no account, no internet needed.

## Features

- Track income and expenses by month
- Set a budget for each category
- Donut charts for actual spending and planned budget
- Budget vs. spent bars for every category
- 6-month income vs. spending chart
- Settings for theme (light, dark, system), accent color, chart colors (including colorblind-safe), font, text size, corner style, and currency
- Sample data button to try it out

## Use it

Download the folder and open `index.html` in any modern browser. That's it.

## Install it as an app (PWA)

In Chrome, Edge, Brave and other Chromium browsers, Tally can be installed and run in its own window, fully offline. Installing needs the app to be served over **HTTPS** or from **localhost**. It won't work from a `file://` address.

- **Online:** host it (see below), open the page, then click the **Install app** button in the header or the install icon in the address bar.
- **Locally:** run `python3 -m http.server 8000` in this folder, open `http://localhost:8000`, and install from there.

Data is stored per address, so a hosted or localhost copy starts with its own empty budget.

## Your data stays with you

Everything is saved in your browser's local storage on your own device. Tally makes no network requests and has no tracking or analytics.

- Clearing your browser's site data erases your budget.
- Data is stored per browser and per file location, so opening the file in a different browser or folder starts fresh.

## Host it (optional)

To put it online with GitHub Pages: push this folder to a GitHub repository, then go to **Settings → Pages**, choose your main branch, and save.

## Hack on it

The app itself is one file, `index.html`: HTML, CSS and plain JavaScript, with no build step and no dependencies. `manifest.webmanifest`, `sw.js` and `icons/` only exist to make it installable. Edit `index.html` and refresh. If you change any file after publishing, bump `CACHE` in `sw.js` so installed copies update.

## License

Public domain, under [The Unlicense](LICENSE). Copy it, change it, sell it, or ignore it. No credit needed.
