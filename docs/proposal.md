# Settle

_AIが会話から割り勘・精算を自動生成し、Solana Payで即決済_

## Summary

Settle is a chat-based AI assistant that reads group conversations (travel, dinners, shared rent) and automatically calculates who owes what, then generates one-tap Solana Pay settlement links in stablecoins. It removes the social friction of asking friends for money by turning natural language into verifiable on-chain payment requests.

## Target users

Friend groups, roommates, travel groups who split expenses frequently

## Problem

Splitting expenses in groups is socially awkward and tracking IOUs across apps is messy and untrustworthy.

## Solution

An AI parses chat/receipts to compute fair splits and issues one-click Solana Pay requests with on-chain settlement history.

## MVP features

- Paste or connect chat log / receipt photo, AI extracts expenses and participants
- Automatic fair-split calculation with custom rules (e.g. exclude non-drinkers)
- Generate Solana Pay QR/link per debtor for instant stablecoin settlement
- On-chain ledger of who paid whom, viewable as a shared group dashboard
- Reminder bot that nudges unpaid members via wallet notification

## Chains

Solana

## Tech

Solana Pay, Rust/Anchor, OpenAI API, Next.js, Phantom Wallet Adapter, USDC

## Category

Payments

## Why now

Solana Pay + stablecoins make instant low-fee settlement finally practical, and LLMs make parsing messy group chats feasible for the first time.

## Roadmap

- Add support for multi-currency and FX-aware splitting
- Integrate with Telegram/Discord bots for native chat workflows
- Partner with stablecoin issuers for cross-border group travel payments
