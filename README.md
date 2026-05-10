# PRRR — Pull Request Review Requests

> Request a review for your pull requests in style.

PRRR is a tiny, zero-dependency tool that generates hilarious PR review nudge messages you can copy and paste into Slack, Teams, email, or wherever your team hides from their notification bell.

No backend. No login. No npm install. Just open `index.html`.

---

## Demo

![PRRR screenshot](https://github.com/PhumudzoSly/prrr/raw/main/screenshot.png)

---

## Features

- **Random messages** — polite nudges or full roast mode, your call
- **Roast mode** — toggle for unhinged, absolutely unfiltered review requests
- **PR link** — paste your PR URL and it gets appended to the copied message
- **One-click copy** — copies message (+ URL if provided) to clipboard instantly
- **Keyboard shortcuts** — `Space` new message · `C` copy · `R` toggle roast
- **100+ messages** — and growing. Contributions welcome

---

## Usage

```bash
git clone https://github.com/PhumudzoSly/prrr.git
cd prrr
open index.html   # or just double-click it
```

That's it. No build step. No dependencies.

---

## Keyboard Shortcuts

| Key     | Action           |
|---------|------------------|
| `Space` | New message      |
| `C`     | Copy to clipboard|
| `R`     | Toggle roast mode|

---

## Project Structure

```
prrr/
├── index.html      # The whole app
├── messages.js     # All the messages — this is where contributions go
└── README.md
```

---

## Contributing

The best way to contribute is to add more messages. The bar is simple: **would your team actually laugh at this?**

### Adding messages

Open `messages.js`. There are two arrays:

- `normalMessages` — polite, passive-aggressive, office-safe nudges
- `roastMessages` — unhinged, chaotic, absolutely not safe for the faint of heart

Add your message to the right array and open a PR.

```js
var normalMessages = [
  // ... existing messages
  "Your new message goes here.",
];
```

### Guidelines

- Keep messages under ~160 characters so they read well in one line
- No slurs, personal attacks, or anything that targets a real person
- Funny > clever > long. If it needs explaining, cut it
- Roast messages should punch at the *code* or the *situation*, not the person

### Other contributions

- **Bug fixes** — open an issue first if it's non-trivial
- **UI improvements** — keep the console aesthetic intact
- **New features** — open an issue to discuss before building

---

## License

MIT — do whatever you want with it. If you use it to shame your teammates into reviewing your PRs, that's on you.

---

Made with frustration and love by [@PhumudzoSly](https://github.com/PhumudzoSly)
