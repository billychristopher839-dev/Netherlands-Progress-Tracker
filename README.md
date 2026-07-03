# 🇳🇱 Nederland: Road to #1

A gamified work/study hour tracker where **you are the Minister-President of the Netherlands**. Govern for **342 completed days** and the Netherlands becomes **#1 in the world for governance**.

## How it works
- **Onboarding (mandatory):** take the oath — your name, a daily hour target, a weekly target, and at least one *portefeuille* (tag). Resetting the game dissolves the government and brings you straight back here.
- **Log your hours:** each session is signed as a *Koninklijk Besluit* (date, duration, tag, note). **Het Wilhelmus plays** every time you log. 🎺
- **Unlock the country:** every day you reach your daily target unlocks **one real gemeente** on the official **2024 municipal map (all 342 of them)** — a grand *Rijkstournee* that starts in **Den Haag**, loops clockwise through all twelve provinces (each opening with its provincial capital), and ends on day 342 in **Amsterdam**. Tap unlocked municipalities to read a true one-line fact about each.
- **Climb the world ranking:** the Netherlands starts **#16**. Roughly every 23 completed days you overtake a rival (Belgium first). **Denmark falls only on day 342.**
- **Streaks & points:** bonuses at 7 / 14 / 30 / 60 / 90 / 180 / 270 / 342 consecutive days. Missed days cost 25 points and reset the streak — but **unlocked gemeenten are never taken away**.
- **Progress tab:** daily (14-day), weekly (8-week) and monthly (6-month) hour charts, plus an immutable *Rijksarchief* of every decree (entries logged today can still be withdrawn).

## Running it
Single self-contained file — the map, the royal seal and the anthem are all embedded.
- Open `index.html` directly, or host it on GitHub Pages.
- Storage: `window.storage` → `localStorage` → in-memory fallback. (Note: `localStorage` needs `https://` or `localhost`; on `file://` some browsers keep data only per-session.)

## Tech notes
- Pure, unit-tested game logic in a `GAME` IIFE (`__GAME_LOGIC_START__` / `__GAME_LOGIC_END__` markers).
- Map: official CBS 2024 gemeente boundaries (SVG), interactive with tooltips, unlock states and a pulsing "next" municipality.
- No external dependencies at load time.

*Je maintiendrai.* 🧡
