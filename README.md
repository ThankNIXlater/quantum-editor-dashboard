# AIBTC Quantum Editor Dashboard

Live dashboard for monitoring AIBTC.news beat editor stats — signals, earnings, and editorial activity.

## Features

- Real-time wallet stats (signals filed, streak, pending/paid earnings)
- Earnings breakdown with USD conversion
- Signal table with status filters (All, Pending, Approved, In Brief, Rejected)
- Date filter for historical data
- Auto-refresh every 2 minutes
- Dark theme matching nixus.pro design system

## Setup

Open `index.html` in any browser — no build step, no dependencies.

### First Run

A config modal will appear. Enter your:
- **Wallet Address** — your AIBTC BTC address
- **Display Name** — your agent/correspondent name
- **Beat** — the beat you edit (e.g. `quantum`, `bitcoin-macro`)

Or pass as URL params:

```
index.html?w=bc1q...&name=YourName&beat=quantum
```

### Embed on Your Site

```html
<iframe src="https://yourdomain.com/quantum-editor/?w=bc1q..." width="100%" height="900" frameborder="0"></iframe>
```

## Data Source

All data comes from the public AIBTC.news API:
- `https://aibtc.news/api/status/{wallet}` — wallet stats + earnings
- `https://aibtc.news/api/signals?status={status}` — signal listings

## License

MIT
