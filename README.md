# 🚀 Times Tables Adventure

> A game-like multiplication trainer for primary school students — built for a real classroom.

**Live demo:** _[Add your GitHub Pages URL here after deployment]_

---

## What it does

Times Tables Adventure turns rote multiplication practice into a game. Students unlock tables one by one (×2 through ×30), answer questions using a big on-screen numpad, and earn progress through speed and accuracy — not just right answers.

Built for a primary school teacher who needed something her students could open on any phone or tablet without creating accounts, downloading apps, or needing Wi-Fi after the first load.

---

## Features

| Feature | Detail |
|---|---|
| 🎮 Game-like progression | Unlock ×2 → ×3 → … → ×30, one at a time |
| 🔐 Unlock system | Need **95% mastery** to unlock the next table |
| ⚡ Speed scoring | Answers under 3 seconds earn full marks; slower answers earn less |
| 🎯 Smart questions | Weakest facts appear most often (spaced-repetition style) |
| 🔢 On-screen numpad | Big tap targets — no device keyboard popup on phones |
| 🌱 Milestone breaks | Celebrations at 25%, 50%, and 75% to keep motivation up |
| 📊 Per-fact tracking | 10 mini progress bars show mastery of each ×1 to ×10 individually |
| 🔥 Streak system | Consecutive correct answers give bonus mastery points |
| 🏆 Session stats | Accuracy, best speed, and best streak shown on completion |
| 🌍 Live user counter | Shows how many students have used the app globally |
| 💾 No account needed | Everything saved in browser localStorage — works offline after first load |
| 📱 Mobile-first | Tested on iPhone SE, Android budget phones, and tablets |

---

## How the scoring works

This isn't simple right/wrong scoring. Each answer is judged on three factors:

1. **Speed** — full score for answers under 3 seconds; zero speed bonus at 15 seconds
2. **Accuracy** — wrong answers cost mastery points (soft penalty when learning, firmer when you should know it)
3. **Consistency** — a streak of correct answers gives bonus points up to +12 per answer

Tables 2–5 progress **1.8× faster** and tables 6–11 progress **1.4× faster** than higher tables, matching how students actually learn (smaller tables are easier and should feel rewarding quickly).

---

## Deploying to GitHub Pages

1. Fork or clone this repository
2. Make sure `index.html` is in the root of your `main` branch
3. Go to **Settings → Pages → Source → Branch: main / (root)**
4. Click **Save** — your site is live at `https://yourusername.github.io/repo-name` in ~30 seconds

That's it. No build step, no dependencies, no server.

> **Note on the user counter:** The live student count uses [CountAPI](https://countapi.xyz/), a free hit-counter service. It only works on HTTPS (deployed) — it will show `100+` when opened locally as a file.

---

## Tech stack

- **HTML / CSS / JavaScript** — single file, zero dependencies
- **Google Fonts** (Nunito) — loaded from CDN
- **CountAPI** — free, backend-free visit counter
- **localStorage** — all progress persisted client-side

No frameworks. No build tools. No npm. Open the file and it works.

---

## Project background

This is a freelance project built for a primary school teacher who wanted her students to practice multiplication tables on classroom tablets and personal phones. Key requirements from the client:

- Must work on cheap Android phones (small screens, slow processors)
- No login, no registration — students just type their name
- Should feel fun, not like a worksheet
- Progress must persist between sessions
- Can be shared as a single link

---

## License

MIT — free to use, modify, and share.

---

_Built with care for a real classroom. Single file, zero setup._
