# Solstream

_Pay-per-second streaming payments for freelancers and creators on Solana_

## Summary

Solstream lets clients pay freelancers, streamers, or API consumers in real-time, per-second micropayments instead of lump sums. It uses Solana's speed and low fees to make continuous payment streams practical, with a simple dashboard to start/stop/monitor streams. Recipients see funds accumulate live and can withdraw anytime.

## Target users

Freelancers, DAOs paying contributors, subscription-based creators, API/SaaS providers

## Problem

Traditional payments are lump-sum and delayed, creating trust issues and cash flow problems for freelancers and continuous services.

## Solution

On-chain payment streaming using Solana programs that release funds continuously, verifiable in real-time by both parties.

## MVP features

- Create a payment stream with rate, token, and duration
- Real-time balance accrual visible to both payer and payee
- Pause/cancel stream with fair pro-rata settlement
- Withdraw accrued funds anytime without waiting for stream end
- Simple embeddable widget for websites to accept streamed payments

## Chains

Solana

## Tech

Anchor, Rust, React, TypeScript, Solana Pay, Phantom Wallet Adapter, Helius RPC

## Category

Payments

## Why now

Solana's sub-second finality and near-zero fees finally make per-second micropayments economically viable, unlike on other chains.

## Roadmap

- Add multi-token support and stablecoin streams
- Integrate with existing freelance platforms via API
- Build recurring/subscription stream templates for SaaS billing
