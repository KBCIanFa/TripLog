# TripLog

# 🚗 Trip Log

A free, private, browser-based road trip journal. Track fuel stops, expenses, and budgets — no account, no cloud, no bullshit.

**[→ Open Trip Log](https://ianfraser.github.io/trip-log/)** <!-- update with your actual URL -->

---

## What it does

- ⛽ **Fuel tracking** — log every fill-up with odometer, litres, price per litre, and location. Calculates L/100km efficiency for each segment automatically.
- 💳 **Expense tracking** — log accommodation, food, activities, camping fees, tolls and more. Categorise, sort, and review everything in one place.
- 📊 **Budget tracker** — set a trip budget and watch a colour-coded progress bar (green → amber → red) track your spend in real time.
- ✏️ **Full edit support** — edit or delete any fuel stop or expense after the fact. Edit trip name, dates, odometer, budget, and notes at any time.
- 📈 **Summary tab** — fuel efficiency chart, spend by category table, and a full trip overview including grand total.
- 💾 **Backup & export** — full JSON backup, fuel CSV, expense CSV, and all-trips summary CSV.
- 📥 **Import** — restore from a backup in merge mode (adds to existing data) or replace mode (full overwrite).
- 🔔 **Auto-backup prompt** — reminds you to download a backup after 10 new entries, with a 24-hour snooze.

---

## Privacy

**All data is stored locally in your browser. Nothing is ever sent to a server.**

There is no backend, no database, no user accounts, and no analytics. Your trip data lives in `localStorage` on your own device. It stays there until you clear your browser data or export it yourself.

This means:
- No sign-up required
- No subscription
- No data collection of any kind
- Works fully offline after the first page load

> ⚠️ Because data is stored in `localStorage`, clearing your browser's site data will erase it. Use the **Download Backup** option regularly to keep a copy safe.

---

## Getting started

1. Open the app in any modern browser
2. Tap **＋ New Trip** and give your trip a name
3. Start logging fuel stops on the **⛽ Fuel** tab
4. Log expenses on the **💳 Expenses** tab
5. Check the **📊 Summary** tab for a live overview

No installation required. Works on iPhone, Android, and desktop.

### Install to home screen (optional)

**iOS (Safari):** Share → Add to Home Screen  
**Android (Chrome):** Menu → Add to Home Screen

---

## Hosting on GitHub Pages

This is a single HTML file with no build step, no dependencies to install, and no server required.

1. Fork or clone this repo
2. Ensure `roadtrip-logger.html` is at the root (or rename it `index.html`)
3. Enable GitHub Pages in **Settings → Pages → Source: main branch / root**
4. Your app will be live at `https://yourusername.github.io/trip-log/`

That's it.

---

## Exporting your data

| Format | Contents | How |
|--------|----------|-----|
| **JSON backup** | All trips, fuel, expenses, categories, settings | Settings → Download Backup |
| **Fuel CSV** | Current trip fuel log | Settings → Download Fuel CSV |
| **Expense CSV** | Current trip expenses | Settings → Download Expense CSV |
| **Summary CSV** | All trips overview | Settings → Download Summary CSV |

Import a JSON backup via **Settings → Import data**. Choose **Merge** to add alongside existing trips, or **Replace** to overwrite everything.

---

## Tech stack

- Vanilla JavaScript — no frameworks, no build pipeline
- Single HTML file — CSS and JS all inline
- `localStorage` for persistence
- DM Sans + DM Serif Display via Google Fonts
- Zero external runtime dependencies

---

## Version history

| Version | Notes |
|---------|-------|
| **v1.1** | Bug fixes: budget bar colour, odometer warning on submit, duplicate total calculation in Summary, backup banner double-call |
| **v1.0** | Initial release — fuel tracking, expense tracking, budget, summary, export/import, edit entries, auto-backup prompt |

---

## Licence

MIT — free to use, modify, and redistribute.

---

Built by [Ian Fraser](https://github.com/ianfraser) · © 2026 <!-- update link -->
