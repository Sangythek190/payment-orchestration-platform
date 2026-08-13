# BYOPG — Zero-Touch Payment Infrastructure

A Product Manager portfolio project demonstrating how I designed a reusable payment automation system that compressed partner onboarding from 24 hours to under 5 minutes.

## Live Demo

[View the interactive demo](https://sangythek190.github.io/byopg-payment-automation/)

## What This Demonstrates

- **Infrastructure Design** — 3 reusable automation actions (Charge Order, Send Invoice, Pay Invoice) powering 3 partners across 3 continents with zero per-partner code
- **Before/After Impact** — 6 manual steps and 24 hours reduced to zero human steps and under 5 minutes
- **Interactive Flow** — Click-through simulation of the webhook-to-activation pipeline
- **Platform Thinking** — One architecture serving multiple payment gateways, currencies, and billing models
- **Market Validation** — Benchmarked against Amplitude 2025 retention data (time-to-first-value under 14 days = 80%+ month-12 retention)

## Northstar Billing Data — Per-Partner Context

| Partner | Paying SMBs | Vendasta Billing | Context |
|---------|-------------|-----------------|---------|
| Zoek | 1,879 | $73K | Revenue contracting — BYOPG is the retention lever that keeps activation friction near zero |
| Telkom | 833 | $62K vendasta billing | $5.7M total monthly revenue — massive scale, PayFast integration unlocks automated billing |
| Italia Online | 2,480 vendasta paying | $32K vendasta billing | Stripe Connect active — BYOPG automation is the next layer |
| Kaseya | 2,137 | $188K | 260% revenue growth — BYOPG success proof: zero-friction billing drives expansion |

## Architecture

```
Partner Payment Gateway
        |
        v
   [Webhook fires]
        |
        v
   Charge Order ──> Send Invoice ──> Pay Invoice ──> AI Products Live
   (match order)    (generate)       (mark paid)     (auto-activate)

   Time: under 5 minutes | Human steps: 0 | Per-partner code: 0
```

## Author

**Sangeetha K** — Product Manager, Integrations & Professional Services

## License

MIT
