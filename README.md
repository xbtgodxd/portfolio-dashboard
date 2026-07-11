# Portfolio Dashboard

### 👉 [Open the dashboard](https://xbtgodxd.github.io/portfolio-dashboard/) — no install, no signup, free

A private, self-contained portfolio tracker that runs entirely in your browser. One HTML file, no server, no account, no tracking — **your financial data never leaves your machine.**

## Why trust it?

- **No backend.** There is no server to send your data to. The entire app is the single `index.html` file in this repository — open it and read every line if you like.
- **Your data stays in your browser.** Positions, notes, and history are stored in your browser's local storage on your device. Nothing is uploaded, ever.
- **What you read is what you run.** The site is served by GitHub Pages directly from this public repository, so the code you can audit here is exactly the code running in your browser.
- **The only network requests are price lookups** (CoinGecko, Binance, Yahoo Finance) and exchange rates — fetched directly from your browser, containing nothing but ticker symbols.

## Features

- **Holdings table** — positions with entry/current price, P&L, allocation, target prices, and leveraged-position support (margin vs. notional, linked cash tracking)
- **Live prices** — automatic price updates for crypto (CoinGecko + Binance cross-check) and stocks (Yahoo Finance), with manual editing always available
- **Multi-currency** — hold assets and cash in 10+ currencies with live FX conversion; pick your home currency and totals show in it alongside USD
- **Net worth history** — monthly snapshots (auto-logged once you start), withdrawal-adjusted performance line, BTC comparison overlay
- **Trade journal** — closed trades with win rate, average win/loss, profit factor, hold time, your original thesis preserved next to the outcome, and CSV export
- **Thesis board** — write down *why* you hold each position, log dated updates, paste chart screenshots
- **Airdrop tracker** — wallets, task checklists, deadlines with alerts, and an allocation calculator
- **Private tab (optional)** — for people who invest through a company: keep the company portfolio and your private economy (home, pension, personal cash) cleanly separated but combined into one net worth
- **Backup & restore** — download your entire dashboard as a single file; restore it anywhere
- **Light & dark themes**, privacy mode (one click hides all amounts), undo/redo, and a renameable title

## Getting started

**Use it online:** open [the hosted page](https://xbtgodxd.github.io/portfolio-dashboard/), click *Add Asset*, and you're tracking. The demo data clears itself as you add your own.

**Or run it locally:** download `index.html` and open it in any browser. It works identically offline (minus live prices).

Either way: click **Backup** now and then. Your data lives in your browser — if you clear browsing data, the backup file is how you get it back.

## Keeping your data safe

- **Backup** (header button) downloads everything as one `portfolio-backup-YYYY-MM-DD.json` file. Keep it somewhere safe.
- **Restore** loads a backup file back in — after a browser reset, on a new machine, or into a newer version of the dashboard.
- Backups are forward-compatible: new versions of the dashboard load old backup files.

## Privacy details, honestly

- Data storage: browser `localStorage`, on your device, tied to this site's address.
- Outbound requests: price quotes (CoinGecko, Binance, Yahoo via a public CORS proxy) and FX rates (open.er-api.com). These requests contain ticker symbols only — never amounts, balances, or notes.
- If you paste chart screenshots into the thesis board, they're stored in your browser too (they're also the main thing that can fill up the ~5 MB storage limit — the dashboard warns you if that happens).

## License

[MIT](LICENSE) — use it, fork it, make it yours.
