# ⛽ Cheapa

**Cheapest fuel prices in Western Australia — live, in your browser.**

Cheapa pulls real-time fuel prices from the WA Government's [FuelWatch](https://www.fuelwatch.wa.gov.au) service, sorts them cheapest-first, and lets you get one-tap directions to any station via Google Maps.

## Features

- 🔴 **Live prices** — updated daily at midnight from FuelWatch WA
- 📍 **GPS detection** — auto-detects your suburb
- ⛽ **All fuel types** — ULP 91, Premium 95/98, Diesel, LPG, E10
- 🗺 **Embedded map** — pins the cheapest station automatically
- 🧭 **One-tap directions** — opens Google Maps with your route ready
- 📊 **Price summary** — cheapest, average, and station count at a glance
- 📱 **Mobile friendly** — responsive layout for phones and tablets

## How it works

```
Browser → rss2json.com (parses FuelWatch RSS) → JSON → Cheapa
```

FuelWatch publishes an RSS feed for every suburb/fuel combination. Since browsers can't fetch it directly (CORS), Cheapa uses [rss2json.com](https://rss2json.com) as a free server-side RSS reader to convert it to JSON.

## Deployment

This is a single static HTML file — no build step, no dependencies, no server required.

Hosted on **GitHub Pages** at: `https://<your-username>.github.io/cheapa`

## Coverage

WA only — FuelWatch is a Western Australian Government service covering Perth metro and regional WA.

## Data source

[FuelWatch WA](https://www.fuelwatch.wa.gov.au) — Western Australian Government  
Prices are set by fuel retailers and locked in each day at midnight.

---

Built with ❤️ for WA drivers.
