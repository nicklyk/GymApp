# 🏋️ GoTrain

A mobile-first workout tracker built as a PWA (Progressive Web App). No installation, no account, no server required. Designed for iPhone Safari and fully installable as a standalone home screen app.

## Features

- **Multiple training plans** — create, copy, edit, rename and delete plans
- **Phases** — organize exercises into color-coded phases (e.g. Warm Up, Strength, Cool Down)
- **Exercise library** — define global exercises with muscle group dropdown and reuse them across plans
- **Two exercise types** — sets/reps or time-based (with countdown timer)
- **Live workout tracking** — check off sets, rest timer between sets, stopwatch per set
- **Next exercise banner** — automatically suggests the next exercise after completing one, including across phases
- **Workout history** — every finished workout is saved with full exercise details (sets, reps, completion status)
- **Abort or finish** — end a workout and save it to history, or abort without saving
- **Export & Import** — back up all data as a `.json` file and restore anytime
- **German & English** — switch language in settings
- **Offline support** — Service Worker caches the app for full offline use
- **PWA ready** — installable via Safari "Add to Home Screen", with custom icon and manifest

## Installation (iPhone)

1. Open the app URL in **Safari**
2. Tap the share icon → **"Add to Home Screen"**
3. The app opens fullscreen like a native app — no address bar, no browser chrome

## Files

| File | Description |
|---|---|
| `index.html` | The complete app (HTML, CSS, JS in one file) |
| `manifest.json` | PWA manifest for app store submission |
| `sw.js` | Service Worker for offline caching |
| `icon-192.png` | App icon 192×192px |
| `icon-512.png` | App icon 512×512px |

All files must be in the same directory for the PWA to work correctly.

## Data Storage

All data (plans, exercises, history, settings) is saved automatically in the browser's `localStorage`. Use **Export** in Settings → General to save a backup `.json` file, and **Import** to restore it.

## App Store Submission

This app is PWA-ready for submission via [PWABuilder](https://pwabuilder.com):

1. Host all files on GitHub Pages
2. Enter your URL at pwabuilder.com
3. Download the generated iOS package
4. Submit via App Store Connect (requires Apple Developer Account, $99/year)

## Tech

Plain HTML, CSS and JavaScript — no frameworks, no build tools, no dependencies. Everything lives in a single `index.html` file (~1700 lines).
