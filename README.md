# Solstream
![Solstream logo](assets/logo.png)

Pay-per-second streaming payments for freelancers and creators on Solana

## Overview

Solstream lets clients pay freelancers, streamers, or API consumers in real-time, per-second micropayments instead of lump sums. Built on Solana, it makes continuous payment streams practical thanks to sub-second finality and near-zero fees. A simple dashboard lets anyone start, stop, and monitor streams, while recipients watch funds accumulate live and withdraw whenever they want.

## Problem

Traditional payments are lump-sum and delayed. A freelancer, streamer, or API provider often has to wait days or weeks to get paid for work that was delivered continuously. This creates trust issues between the parties and real cash flow problems for the people providing ongoing value.

## Solution

Solstream uses on-chain payment streaming powered by a Solana program. Instead of a single transfer at the end of a job or billing period, funds are released continuously and are verifiable in real time by both the payer and the payee. The payee's balance grows every second, and either side can end the arrangement fairly at any time.

## Features (MVP)

- Create a payment stream with a chosen rate, token, and duration
- Real-time balance accrual visible to both payer and payee
- Pause or cancel a stream with fair, pro-rata settlement
- Withdraw accrued funds anytime, without waiting for the stream to end
- Simple embeddable widget for websites to accept streamed payments

## Tech Stack

- Anchor + Rust for the on-chain Solana program
- React + TypeScript for the dashboard and widget
- Solana Pay for payment interactions
- Phantom Wallet Adapter for wallet connection
- Helius RPC for reliable Solana network access

## How It Works

```
Payer (Dashboard) --create stream--> Anchor Program (Solana)
                                        |
                                per-second accrual
                                        |
Payee (Dashboard/Widget) <--withdraw-- Anchor Program
```

1. The payer creates a stream on-chain, specifying rate, token, and duration.
2. The Anchor program locks the funds and continuously computes the accrued balance based on elapsed time.
3. Both payer and payee see the live balance in the dashboard.
4. The payee can withdraw accrued funds at any time.
5. Either party can pause or cancel the stream; the program settles the remaining balance pro-rata.

## Roadmap

- Add multi-token support and stablecoin streams
- Integrate with existing freelance platforms via API
- Build recurring/subscription stream templates for SaaS billing

## Pitch

See our one-page pitch deck at [docs/pitch.pdf](docs/pitch.pdf) and the spoken pitch script at [docs/pitch-script.md](docs/pitch-script.md).

## Team

- [Name] - Role - [GitHub/Twitter]
- [Name] - Role - [GitHub/Twitter]
- [Name] - Role - [GitHub/Twitter]

Built for the Colosseum hackathon.

---

🎬 Pitch video: [docs/pitch-video.mp4](docs/pitch-video.mp4)
