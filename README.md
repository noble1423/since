# Since

*for the things that quietly wait*

Since is a small, calm app for tracking how long it's been since you last did the things you tend to forget — calling someone you love, watering the plant, changing the sheets, checking the smoke alarm.

No due dates. No streaks. No red notification badges guilting you. Just an honest, ambient sense of "how long has it actually been," so your attention naturally goes where it's needed.

## How it works

- Each thing you're keeping an eye on gets a card with a live counter — days and hours since you last did it.
- Tap **Done today** and the counter resets with a soft flip animation.
- Cards are colored calmly (fresh → getting old → overdue) based on your own rough sense of how often something needs doing — no strict deadlines.
- Cards automatically sort so whatever's relatively most overdue rises to the top.
- Add your own items with an emoji, a name, and a loose cadence like "about a week" or "every few months."

## Accounts

Since includes simple sign up / sign in so more than one person can use the same device or the same deployed page, each with their own private list.

- Passwords are hashed (SHA-256 with a random salt) before being stored — reasonable for casual use, but **not** something to reuse a sensitive password on.
- Accounts and lists are saved using your browser's `localStorage`. That means:
  - Your data stays **on this device, in this browser** — it won't sync to your phone or a different browser automatically.
  - Clearing your browser's site data will erase it.
  - There's no server, so nobody but someone using this exact browser can see it.

## Running it yourself

This is a single self-contained HTML file — no build step, no dependencies.

**Locally:**
Just open `since.html` (or `index.html`) in a browser.

**On GitHub Pages:**
1. Push this file to a repo (rename it to `index.html` if you want it at the root).
2. Go to **Settings → Pages**, set the source to your branch and root folder.
3. Your app will be live at `https://<your-username>.github.io/<repo-name>/`.

GitHub Pages serves over HTTPS by default, which this app needs for password hashing to work correctly.

## Limitations

- No cross-device sync — accounts and data live in one browser's local storage.
- Not intended for sensitive passwords or sensitive data.
- No password recovery — if you forget it, you'll need to create a new account.

## Built with

Plain HTML, CSS, and JavaScript. Fonts: [Fraunces](https://fonts.google.com/specimen/Fraunces), [IBM Plex Sans](https://fonts.google.com/specimen/IBM+Plex+Sans), and [IBM Plex Mono](https://fonts.google.com/specimen/IBM+Plex+Mono) via Google Fonts.
