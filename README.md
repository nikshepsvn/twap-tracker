# TWAP Flow — Hyperliquid

Live [Hyperliquid](https://hyperliquid.xyz) TWAP order flow, aggregated by token. See net buying / selling pressure across perps, spot, and builder DEXes in real time.

**Live:** https://nikshepsvn.github.io/twap-tracker/

## What it does

- Pulls all recent TWAP orders from [hypurrscan](https://hypurrscan.io) and resolves asset names + current mark prices from the Hyperliquid API.
- Aggregates by token: order counts, live (currently executing) count, buy/sell sizes, and **net notional flow**.
- Net-flow chart, sortable table, status/window/unit filters, and per-token drill-down with live TWAP progress bars and countdowns.

## Stack

Single static `index.html` — no backend, no build step. All data is fetched client-side from public APIs, so it hosts free on GitHub Pages.

## Run locally

Just open `index.html` in a browser, or serve it:

```sh
python3 -m http.server
```
