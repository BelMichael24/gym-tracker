# 🏋️‍♂️ Jacked.

> A lightweight, offline-first Progressive Web App (PWA) to track your workout sessions, track strength progression over time, and celebrate personal records (PRs) — with zero fluff and full data ownership.

---

## ⚡ Features

- 📱 **Progressive Web App (PWA):** Install it on iOS or Android directly from your browser.
- 🔒 **Privacy-First & Offline-First:** All data stays local on your device via `localStorage`. No login, no cloud dependency, no trackable data.
- 🏆 **Automatic PR Detection:** Automatically calculates $1\text{RM}$ (One Rep Max) estimations using the Epley formula and highlights Personal Records on session summaries.
- 🎨 **11 Creative Themes:** Fully customizable color palettes ranging from Cyberpunk Amber, Vampire Red, Synthwave, Electric Cyber (AMOLED), to Matrix Lime.
- 📅 **Interactive Progress Calendar:** Tap any date to view, edit, or delete logged workout history.
- 📈 **Dynamic Strength Charts:** Visual graph tracking of estimated $1\text{RM}$ progress across exercises over time.
- ➕ **Smart Weight & Rep Steppers:** Quick increment/decrement controls ($\pm 2.5\text{ kg}$ for weights, $\pm 1$ for reps) optimized for mobile logging.
- 💾 **Data Backup & Restore:** Easily export your entire history as a JSON payload to back up or migrate across devices.

---

## 🚀 Getting Started

### Option 1: Direct File Usage (Zero Setup)
1. Download the `index.html` file.
2. Double-click to open it in any modern web browser (Chrome, Safari, Firefox, Edge).
3. Start logging!

### Option 2: Host via GitHub Pages
1. Push `index.html` to your GitHub repository.
2. Go to **Repository Settings** $\rightarrow$ **Pages**.
3. Under **Source**, select `main` (or `master`) branch and click **Save**.
4. Open the generated site URL on your mobile browser and tap **"Add to Home Screen"** to install as a PWA.

---

## 📊 How PRs Are Calculated

Estimated One-Rep Max ($1\text{RM}$) is calculated automatically for each set using the Epley formula:

$$1\text{RM} = \text{Weight} \times \left(1 + \frac{\text{Reps}}{30}\right)$$

When saving a workout, the app compares the top estimated $1\text{RM}$ of the session against all historical entries for that exercise. If exceeded, a **🏆 PR** badge is awarded!

---

## 🎨 Available Themes

Toggle between 11 vibrant themes in the **Settings (⚙)** menu:

| Theme Name | Style / Aesthetic |
| :--- | :--- |
| **Cyberpunk Amber** | Warm amber on dark chocolate |
| **Electric Cyber (AMOLED)** | Neon cyan on pitch black |
| **Vampire Red** | Crimson highlight on deep dark red |
| **Retro Synthwave** | Purple & hot pink (Dracula inspired) |
| **Deep Moss Green** | Natural forest green tones |
| **Glacier Ice Blue** | Cool icy blue palette |
| **Toxic Hacker Lime** | High-contrast green on dark slate |
| **Solar Flare Orange** | Energetic fiery orange |
| **Midnight Amethyst** | Deep violet & purple hues |
| **Gunmetal Steel** | Modern slate grey |
| **Neon Dusk Coral** | Sunset pink & coral tones |

---

## 🛠️ Tech Stack

- **HTML5 & CSS3:** Native CSS variables for real-time theme swapping.
- **Vanilla JavaScript (ES6+):** Zero external libraries or frameworks for fast rendering.
- **HTML5 Canvas:** Custom light-weight charting engine built from scratch.
- **Web Storage API:** Local persistent state management via `localStorage`.

---

## 🛠️ Data Backup & Migration

To back up your data or switch devices:
1. Tap the **Settings (⚙)** icon in the header.
2. Click **Backup Data** to copy your complete workout history and settings to your clipboard.
3. On your new device, open the app, navigate to **Settings**, click **Restore Data**, and paste the backup snippet.

---

## 📄 License

This project is licensed under the **MIT License** — feel free to modify, distribute, or host your own instance!
