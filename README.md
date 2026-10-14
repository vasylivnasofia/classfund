# ClassFund

A transparent class fund for parents.

In many schools, parents pay a monthly contribution for class needs like repairs, gifts and trips. One parent collects the cash, and the others rarely see where it goes. ClassFund puts the class fund in one shared wallet. Every payment in and every purchase out is recorded on Solana with a photo of the receipt. Large purchases need approval from other parents before any money moves.

> **Status: MVP prototype.** This repo contains a clickable user-experience prototype. Balances, families, receipts and votes are mock data. No wallet connects and no money moves.

## Try it

Open `index.html` in a browser, or visit the GitHub Pages site once it's enabled.

- **Overview**: class balance, who has paid this month, and any open vote
- **Ledger**: every payment in and out, each with its receipt
- **Votes**: approve or reject a large purchase, such as a new projector
- **Pay**: pay the monthly contribution by card and see it land in the class wallet

## Project structure

```
classfund/
├── index.html          # App markup: phone frame, four screens, tab bar
├── css/
│   └── styles.css      # Styles, light and dark theme
├── js/
│   ├── data.js         # Mock data: balance, families, ledger, open vote
│   ├── utils.js        # Helpers: DOM lookup, formatting, navigation, toasts
│   └── app.js          # Screens and interactions
└── docs/
    ├── ARCHITECTURE.md # How the prototype works and the planned on-chain design
    └── ROADMAP.md      # What comes after the prototype
```

No build step and no dependencies. The scripts are plain JavaScript loaded in order, so the app also runs straight from the file system.

## Deploy to GitHub Pages

1. Push this repo to GitHub.
2. Go to **Settings → Pages**.
3. Choose **Deploy from a branch**, select `main` and `/ (root)`, and save.
4. The site appears at `https://<your-username>.github.io/<repo-name>/`.

## License

MIT. See [LICENSE](LICENSE).
