# 🩺 Tlak - Blood Pressure Journal PWA

> A minimalist, offline-first Progressive Web App for daily blood pressure tracking - built for real personal use, installable without any app store.

![PWA](https://img.shields.io/badge/PWA-ready-7c6dfa?style=flat-square)
![License](https://img.shields.io/badge/license-MIT-6bffb8?style=flat-square)
![Lang](https://img.shields.io/badge/lang-CS%20%2B%20EN-4ecdc4?style=flat-square)
![Vanilla JS](https://img.shields.io/badge/built%20with-Vanilla%20JS-ff6b6b?style=flat-square)

---

## Motivation

My doctor asked me to track my blood pressure every morning for a few weeks and bring a summary to the next appointment. Every app I found was either bloated with ads, required account registration, or sent my health data to some server I didn't ask about.

So I built (1st vibecoded app) this instead - a single HTML file that lives on GitHub Pages, installs like a native app on Android, works completely offline, and exports a clean CSV when it's time for the appointment. No backend. No tracking. No nonsense.

---

## Features

- **Daily logging** - systolic / diastolic input with instant BP category feedback
- **Visual history** - 14-day chart rendered on raw Canvas (no chart libraries)
- **Statistics** - average, max, min across all recorded entries
- **CSV export** - bilingual (CS + EN) table ready to hand to a doctor
- **Offline support** - Service Worker caches the app on first load
- **Installable** - full PWA manifest, adds to home screen like a native app
- **Bilingual UI** - Czech primary, English secondary throughout
- **Zero dependencies** - no frameworks, no npm, no build step. One HTML file.

---

## Tech

| What | How |
| --- | --- |
| UI | Vanilla JS, CSS custom properties |
| Chart | HTML5 Canvas API |
| Storage | `localStorage` |
| Offline | Service Worker + Cache API |
| Fonts | Google Fonts (Space Mono + Syne) |
| Hosting | GitHub Pages |
| Build step | None |

---

## Getting Started

No installation needed. Just open the live app:

**[→ Live App](https://chief1y.github.io/Blood-pressure-helper/)**

Or run locally - just open `index.html` in any browser. No server needed.

### Deploy your own copy

```bash
git clone https://github.com/Chief1y/Blood-pressure-helper.git
cd tlak
# open index.html - done
```

To deploy to GitHub Pages:

1. Fork this repo
2. Go to **Settings → Pages → Source: main / root**
3. Your instance is live at `https://YOUR_USERNAME.github.io/tlak`

### Install on Android

1. Open the live URL in **Chrome**
2. Tap ⋮ → **Add to Home Screen**
3. Done - works offline, icon on home screen

---

## BP Categories

Standard ESH/ESC classification:

| Category | Systolic | Diastolic |
| --- | --- | --- |
| ✅ Normal / Normální | < 120 | < 80 |
| ⚠️ Elevated / Zvýšený | 120-129 | < 80 |
| 🟠 Hypertension 1° / Hypertenze 1° | 130-139 | 80-89 |
| 🔴 Hypertension 2° / Hypertenze 2° | ≥ 140 | ≥ 90 |

---

## Privacy

All data is stored locally in your browser's `localStorage`. Nothing is sent anywhere. No analytics. No cookies. No server.

---

## License

MIT — see [LICENSE](./LICENSE)

You're free to use and modify this project, but **you must keep the original author credit**. You may not claim this as your own original work.

---

## Author

Built by **chief1y** · [github.com/Chief1y](https://github.com/Chief1y)

*CS student at FIT VUT Brno · part-time automation developer*

---

<sub>Yes, I track my blood pressure now. Getting old is fun.</sub>
