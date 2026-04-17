<p align="center">
  <a href="https://github.com/Chris0x88">
    <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&size=26&duration=3500&pause=800&color=58A6FF&center=true&vCenter=true&width=760&lines=Trained+in+engineering+and+law.+Writing+software+now.;Autonomous+trading.+Edge+compute.+Self-custody.;Keys+on+your+machine.+No+rent%2C+no+middle-layers.;Hedera+%C2%B7+Hyperliquid+%C2%B7+Python+%C2%B7+Claude+Code" />
  </a>
</p>

<p align="center">
  <a href="https://chris0x88.github.io"><img src="https://img.shields.io/badge/Portfolio-0b1020?style=for-the-badge&logo=vercel&logoColor=58a6ff"></a>
  <a href="https://huggingface.co/Chris0x88"><img src="https://img.shields.io/badge/HuggingFace-FFD21E?style=for-the-badge&logo=huggingface&logoColor=black"></a>
  <a href="mailto:rhczs6bz4d@privaterelay.appleid.com"><img src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white"></a>
</p>

---

## What I build

> Engineering and law before code. I came to software with the habit of specifying things before building them, and treating a live system like something that can actually hurt you. Now I build autonomous trading agents, risk systems, and direct-to-chain SDKs — software that acts on its own but is designed to be argued with, not trusted blindly.
>
> **Principle I keep coming back to:** slash commands are cheap deterministic code, AI is expensive judgment. Don't confuse the two. Every system below reflects that split.

## Flagship projects

### [hyperliquid-agent](https://github.com/Chris0x88/hyperliquid-agent) — *An AI trading co-pilot that lives inside your Hyperliquid client*

<img src="assets/logos/hyperliquid-agent.png" width="120" align="right" alt="hyperliquid-agent"/>

Not a bot that trades for you — a partner that sits beside you while you do. Reads your positions, your thesis, and your risk. Drafts stop losses and take profits from the signals and market structure you actually care about. Bounces ideas, argues the other side, questions you when you scale leverage past what the thesis supports. Carries the ugly operational work — account state, trailing stops, profit locking — so the trader can stay on the trade.

Built by porting Claude Code's agent runtime into the trading loop itself. Free-text routes to the embedded agent; fixed commands stay fast, deterministic, and zero-credit. Keys dual-written to an AES-256-GCM vault and macOS Keychain. API wallets only — a leaked key can't withdraw.

<br clear="right"/>

### [Space Lord](https://github.com/Chris0x88/spacelord) — *Your Hedera wallet, exchange, and trading desk collapsed into one local CLI*

<img src="assets/logos/spacelord.png" width="120" align="right" alt="Space Lord"/>

Built for the **2026 Hedera Apex Hackathon** as the execution surface for an [OpenClaw](https://openclaw.ai) AI agent. Core design goal was raw edge compute — no third-party APIs between the agent and the chain. Own-rolled comms straight to Hedera mainnet rather than piping through middleware that could rate-limit, go down, or rug the API layer.

The agent drives everything through **CLI tool use, not MCP**: one valid execution path per operation, so the LLM can't invent a swap. Governance is read-only config the agent can't edit (per-swap caps, daily caps, slippage ceilings). Gets faster again once BlockStreams rolls out on Hedera.

<br clear="right"/>

### [AusFuelWatch](https://github.com/Chris0x88/AUS_FUEL_WATCH) — *A live map of the ships carrying Australia's fuel*

<img src="assets/logos/ausfuelwatch.png" width="120" align="right" alt="AusFuelWatch"/>

Built during the March 2026 fuel crisis. Three localhost processes — an AIS WebSocket proxy, a Claude-powered intel server, and a standalone HTML dashboard — no backend, no login, no web server. The dashboard opens from the filesystem.

The Singapore corridor vessel count is the leading indicator for Australian pump prices, so the whole thing exists to watch it. Terrestrial AIS has no coverage across the open Indian Ocean, so tanker departures are detected by snapshot diff rather than live feed.

<br clear="right"/>

### [power-law-allocation](https://github.com/Chris0x88/power-law-allocation) — *A Bitcoin allocation model that decides the BTC/cash split for you*

<img src="assets/logos/power-law-allocation.png" width="120" align="right" alt="power-law-allocation"/>

Same date and price in, same signal out. No database, no historical feed, no ML — just a power law, Kleiber's Law, and a heartbeat. ~400-line core, zero I/O, runs in a Lambda. Ships with a venue-agnostic rebalancer.

**The finding that matters:** a rebalance threshold of **15% or more** is where this strategy earns its keep. Go tighter and fees, slippage, and tax drag eat the edge faster than rebalancing creates it. Bitcoin swings 15% often enough that each time it does, you bank another chunk of value. Five locked constants. I won't tune them — that's the point.

<br clear="right"/>

### [saucerswap-python-sdk](https://github.com/Chris0x88/saucerswap-python-sdk) — *A direct line from an AI agent to SaucerSwap*

<img src="assets/logos/saucerswap-python-sdk.png" width="120" align="right" alt="saucerswap-python-sdk"/>

Production Python SDK that talks to the SaucerSwap V2 router contracts directly rather than hitting the public API. Built for AI agents that need a deterministic, always-on line into Hedera DeFi — no rate limits, no middleware outages, no API layer that can break between you and the trade. Runs my own trading stack and is available for anyone building an agent that needs the same.

<br clear="right"/>

---

## How I work

Bias toward small, readable systems that survive the 3am weekend stop-hunt. Keys on disk, code on GitHub, nothing phoning home. Where an LLM helps, it gets a fixed tool surface; where it doesn't, there's a deterministic command. I'd rather ship a 400-line model I understand than a framework I don't.

## Stack

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![Claude Code](https://img.shields.io/badge/Claude_Code-D97757?style=for-the-badge&logo=anthropic&logoColor=white)
![Hedera](https://img.shields.io/badge/Hedera-222222?style=for-the-badge&logoColor=white)
![Hyperliquid](https://img.shields.io/badge/Hyperliquid-50D2C1?style=for-the-badge)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)


---

<sub>📬 <a href="mailto:rhczs6bz4d@privaterelay.appleid.com">rhczs6bz4d@privaterelay.appleid.com</a> · 🌐 <a href="https://chris0x88.github.io">portfolio</a> · 🐙 <a href="https://github.com/Chris0x88">github.com/Chris0x88</a> · 🤗 <a href="https://huggingface.co/Chris0x88">huggingface.co/Chris0x88</a></sub>
