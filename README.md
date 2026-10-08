# Settle
![Settle logo](assets/logo.png)

AIが会話から割り勘・精算を自動生成し、Solana Payで即決済

## Overview
Settle is a chat-based AI assistant that reads group conversations about travel, dinners, or shared rent, automatically calculates who owes what, and generates one-tap Solana Pay settlement links in stablecoins. It turns natural language into verifiable, on-chain payment requests.

## Problem
Splitting expenses in groups is socially awkward, and tracking IOUs across multiple apps and screenshots is messy and untrustworthy. People forget, delay, or avoid asking friends for money.

## Solution
Settle's AI parses chat logs or receipt photos to extract expenses and participants, computes a fair split (with custom rules like excluding non-drinkers), and issues a Solana Pay QR code or link for each debtor. Every settlement is recorded on-chain, creating a shared, trustworthy group ledger.

## Features (MVP)
- Paste or connect a chat log, or upload a receipt photo; AI extracts expenses and participants
- Automatic fair-split calculation with custom rules
- Generate a Solana Pay QR/link per debtor for instant stablecoin settlement
- On-chain ledger of who paid whom, viewable as a shared group dashboard
- Reminder bot that nudges unpaid members via wallet notification

## Tech Stack
- Solana Pay for payment requests
- Rust / Anchor for on-chain programs
- OpenAI API for chat/receipt parsing
- Next.js for the web app
- Phantom Wallet Adapter for wallet connection
- USDC as the settlement stablecoin

## How It Works
```
Chat log / receipt photo
        |
        v
  AI parsing (OpenAI API)
        |
        v
 Fair-split calculation engine
        |
        v
Solana Pay link/QR per debtor
        |
        v
  On-chain settlement (Solana)
        |
        v
 Shared group dashboard + reminders
```

## Roadmap
- Add support for multi-currency and FX-aware splitting
- Integrate with Telegram/Discord bots for native chat workflows
- Partner with stablecoin issuers for cross-border group travel payments

## Pitch
- [Pitch deck (PDF)](docs/pitch.pdf)
- [Pitch script](docs/pitch-script.md)

## Team
- [Name] — Role (placeholder)
- [Name] — Role (placeholder)
- [Name] — Role (placeholder)

Built for the Colosseum hackathon (Solana and other chains).

---

🎬 Pitch video: [docs/pitch-video.mp4](docs/pitch-video.mp4)


## Prototype

Live prototype: https://rairaisann.github.io/settle/

The source is [docs/index.html](docs/index.html) (served with GitHub Pages from the /docs folder). All data is simulated.

🎥 Demo video: [docs/demo-video.mp4](docs/demo-video.mp4)
