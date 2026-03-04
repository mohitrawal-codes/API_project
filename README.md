# 🌍 Place Explorer

> Search any place in the world — get live weather, location info, historical facts, and a live local clock.

**Live demo → [your-username.github.io/place-explorer](https://your-username.github.io/place-explorer)**

---

## Features

- 🌤 **Live weather** — temperature, humidity, wind, pressure, visibility
- 📍 **Location info** — coordinates, timezone, population, area, elevation, currency
- 📜 **Historical facts** — 5 curated facts about the place
- ✦ **About this place** — rich cultural description
- 🕐 **Live local clock** — ticking in the place's real timezone
- ✏️ **Typo correction** — "Mumbay" → Mumbai, "Paries" → Paris
- 🗺️ **Smart errors** — unrecognised places get friendly suggestions

---

## Setup

### 1. Get a free OpenWeatherMap API key
Sign up at [openweathermap.org](https://openweathermap.org/api) — the free tier is enough.

> ⚠️ New keys take **up to 2 hours** to activate after creation.

### 2. Paste your key into `index.html`
Open `index.html` and find line ~60:
```js
const OWM_KEY = "YOUR_OWM_KEY_HERE";
```
Replace `YOUR_OWM_KEY_HERE` with your actual key.

### 3. Run locally
Just open `index.html` in any browser — no server needed.

---

## Deploy to GitHub Pages (free hosting)

1. Create a new GitHub repository called `place-explorer`
2. Upload `index.html` and `README.md`
3. Go to **Settings → Pages → Source → main branch → / (root)**
4. Click **Save** — your site will be live at:
   ```
   https://your-username.github.io/place-explorer
   ```

---

## Tech Stack

| Layer | Technology |
|-------|-----------|
| UI | React 18 (CDN, no build step) |
| Styling | Plain CSS |
| AI (place info, validation) | Claude API (claude-sonnet-4) |
| Weather | OpenWeatherMap API |
| Hosting | GitHub Pages |

---

## Project Structure

```
place-explorer/
└── index.html    ← entire app in one file
└── README.md
```

---

*Built with Claude AI + OpenWeatherMap*
