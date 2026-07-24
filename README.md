# Hangman — Android App

A classic Hangman word-guessing game built for Android. Tap letters to guess the hidden word before the man is hanged. Clean dark UI, fully touch-optimised, no internet connection required after install.

**Designed by Scientist47**

---

## Screenshots

> Add your screenshots here after installing the app.

---

## Download & Install

### Option A — Install the APK directly

1. Download `hangman.apk` to your Android phone
2. Go to **Settings → Apps → Special App Access → Install Unknown Apps**
3. Allow your file manager or browser to install APKs
4. Tap the `.apk` file and select **Install**
5. Open **Hangman** from your app drawer

> Android 8.0 and above is required.

### Option B — Play in your browser (no install needed)

Open the link below in any mobile browser and play instantly:

```
https://yourusername.github.io/hangman
```

Replace `yourusername` with your actual GitHub username.

---

## How to Play

1. A secret word is chosen and shown as blank letter tiles
2. Tap any letter on the keyboard to guess it
3. A correct guess reveals the letter in the word
4. A wrong guess costs one life and adds a body part to the scaffold
5. You have **6 lives** — use them wisely
6. Guess the full word before all 6 lives are gone to win
7. Tap **NEW GAME** at any time to start a fresh round

---

## Features

- 35+ built-in words across different categories
- Animated letter reveals
- Live lives counter
- Full keyboard with hit/miss colour feedback
- Works completely offline after install
- Optimised for all Android screen sizes
- Physical keyboard supported (for tablets and Chromebooks)

---

## Project Files

```
hangman-android/
├── hangman.html        # Full game source (HTML + CSS + JS, single file)
├── README.md           # This file
```

The entire game lives in one self-contained HTML file. No frameworks, no dependencies, no build tools.

---

## How the APK Was Built

The app is a web wrapper around `hangman.html`, hosted on GitHub Pages and packaged using **WebIntoApp**.

### Step 1 — Host on GitHub Pages

1. Create a repository on [github.com](https://github.com)
2. Upload `hangman.html` and rename it `index.html`
3. Go to **Settings → Pages → Branch: main → Save**
4. Game is live at `https://yourusername.github.io/hangman`

### Step 2 — Generate the APK

1. Go to [webintoapp.com](https://webintoapp.com)
2. Paste your GitHub Pages URL
3. Set app name to **Hangman** and author to **Scientist47**
4. Download the `.apk` file

### Step 3 — Install on Android

Follow the **Option A** steps above.

---

## Customising the Word List

Open `hangman.html` in any text editor. Find this section near the bottom:

```javascript
const WORDS = [
  "python", "javascript", "hangman",
  // add your words here
];
```

Rules for adding words:
- Lowercase letters only
- No spaces, numbers, or special characters
- Minimum 4 letters recommended for a fair game

Save the file, re-upload to GitHub Pages, and the app updates automatically on next launch.

---

## Rebuilding After Changes

If you change `hangman.html` and want a fresh `.apk`:

1. Push the updated file to your GitHub repository
2. Wait ~60 seconds for GitHub Pages to refresh
3. Go back to [webintoapp.com](https://webintoapp.com) and regenerate the APK

---

## Troubleshooting

| Problem | Fix |
|---|---|
| "App not installed" error | Enable **Install Unknown Apps** in Settings |
| App won't open after install | Restart your phone and try again |
| Blank screen on launch | Check your internet connection (first launch loads the hosted page) |
| Letters too small to tap | Increase font size in Android Accessibility settings |
| Want to play offline fully | Open `hangman.html` directly in Chrome on your phone |

---

## Tech Stack

| Layer | Technology |
|---|---|
| Game logic | Vanilla JavaScript |
| UI | HTML5 + CSS3 |
| Fonts | Courier New (system font, no download) |
| Hosting | GitHub Pages (free) |
| APK wrapper | WebIntoApp (free) |

---

## Licence

Free to use and modify for personal and educational projects.

---

*Designed by Scientist47*
