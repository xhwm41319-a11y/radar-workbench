# RADAR Workbench 🛰️
### The Open-Source, Local-First Smart Money & Whale Radar for Solana
> **Catch Raydium & Pump.fun DEX liquidity launches and whale swaps with 0 cloud latency. Flag malicious Token-2022 honeypots before you trade. 0 paid API keys required.**

[![Solana](https://img.shields.io/badge/Solana-Mainnet-9945FF?style=flat&logo=solana&logoColor=white)](https://solana.com)
[![Token-2022](https://img.shields.io/badge/Standard-Token--2022-14F195?style=flat)](https://spl.solana.com/token-2022)
[![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](LICENSE)
[![Latest Release](https://img.shields.io/github/v/release/xhwm41319-a11y/radar-workbench?color=orange&label=Release)](https://github.com/xhwm41319-a11y/radar-workbench/releases/tag/v0.3.4)
[![YouTube Demo](https://img.shields.io/badge/YouTube-2--Min_Demo-red?style=flat&logo=youtube&logoColor=white)](https://youtu.be/zJyeauPnAns)
[![Telegram Lab](https://img.shields.io/badge/Community-Telegram_Lab-2CA5E0?style=flat&logo=telegram&logoColor=white)](https://t.me/sol_alpha_radar_lab)
[![Twitter](https://img.shields.io/badge/X-@radraw6o-black?style=flat&logo=x&logoColor=white)](https://x.com/radraw6o)

---

### [👉 Download Latest Offline Workbench (v0.3.4) — Free & Open Source](https://github.com/xhwm41319-a11y/radar-workbench/releases/tag/v0.3.4) | [▶️ Watch Video Walkthrough](https://youtu.be/zJyeauPnAns)

---

## ⚡ Why RADAR? (Comparison vs Cloud SaaS)

Most Solana traders and snipers rely on cloud web dashboards or Telegram bots. By the time an alert pops up on your screen, cloud queuing and indexing lag have already eaten your edge.

| Feature | RADAR Workbench (Local-First) | Cloud Web Dashboards (DexScreener, Photon) | Paid Alpha Telegram Bots ($100+/mo) |
| :--- | :--- | :--- | :--- |
| **Latency** | **Sub-second (Direct RPC WebSocket)** | 3 – 15s indexing delay | 2 – 8s message queue delay |
| **Token-2022 Trap Inspection** | **✅ Deep Bytecode & Hook Check** | ⚠️ Generic or delayed score | ❌ Basic mint freeze only |
| **Privacy & Security** | **🔒 100% Local / Zero Wallet Connect** | ⚠️ Web tracking & cloud telemetry | ⚠️ Telegram bot custody / token exposure |
| **Cost** | **Free & Open-Source (Apache 2.0)** | Free (ad-supported / rate-limited) | $50 – $300 / month |
| **Network Reliance** | **Runs offline or with any RPC** | Centralized web servers | Centralized bot servers |

---

## 🛰️ Overview / 概述

**RADAR Workbench** is an open-source, deterministic on-chain risk telemetry and smart money tracking suite for Solana traders, security researchers, and automated AI agents.

Instead of vague "trust-me" black-box security scores, RADAR analyzes raw on-chain instruction bytecode, exact block slots, freeze authority boundaries, and smart money token flows directly into self-contained, auditable evidence cards.

**RADAR** 为 Solana 链上交易员、安全研究员及自动化 AI 代理提供透明、可验证的风险遥测。区别于黑盒审计评分，RADAR 将链上指令集、确切时间槽（Slot）、冻结权限边界及未知项生成为完全独立的离线证据卡片。

![RADAR Workbench Preview](docs/preview-en.png)

---

## 🛡️ Core Capabilities / 核心特性

* **🔍 Token-2022 Exploit Detection**: Instant bytecode inspection for malicious `Permanent Delegate`, `Default Account Freeze`, and hidden `Transfer Fee` hooks before you swap.
* **📊 Local-First Offline Workbench (v0.3.4)**: Zero npm dependencies, zero remote tracking, zero wallet/private key exposure. Runs 100% inside your browser engine.
* **⚡ Sub-Second Liquidity Telemetry**: Listen directly to Raydium AMM / CLMM and Pump.fun liquidity creation events via raw RPC WebSocket without third-party API bottlenecks.
* **⚖️ Standalone Order & Payment Reconciliation (v0.2.1)**: Local utility for matching on-chain transactions against internal order records without exposing database credentials.
* **📑 Deterministic Evidence Cards**: Import standard Solana `getBlock` JSON data, parse account co-occurrences, and export shareable, zero-script HTML evidence cards.

---

## 🚀 Quick Start / 快速开始 (10 Seconds)

### 1. Download Latest Release
Navigate to GitHub Releases or download directly:
* **[RADAR-Research-Workbench-0.3.4.zip](https://github.com/xhwm41319-a11y/radar-workbench/releases/tag/v0.3.4)** — Standalone research review workbench (`SHA256: de5174bf...`)
* **[RADAR-Order-Reconciliation-0.2.1.zip](https://github.com/xhwm41319-a11y/radar-workbench/releases/tag/v0.3.4)** — Local order mismatch reviewer (`SHA256: 7a0cc9be...`)

### 2. Run Locally (No Server / No Build Required)
Extract the archive and open the HTML interface directly in any modern browser:
```bash
unzip RADAR-Research-Workbench-0.3.4.zip
cd RADAR-Research-Workbench-0.3.4
open research-review.html
```
1. Click **"Load Demo"** or import any standard Solana block / transaction JSON file.
2. Review structured findings: Slot range, coverage bounds, and potential honeypot flags.
3. Click **"Export HTML"** to produce an auditable, self-contained report card.

---

## ❓ Frequently Asked Questions (FAQ)

<details>
<summary><b>Do I need to connect my Solana wallet or share private keys?</b></summary>
<p><b>Never.</b> RADAR is strictly read-only and local-first. It never asks for, handles, or stores private keys, seed phrases, or signatures.</p>
</details>

<details>
<summary><b>Do I need expensive paid RPC endpoints (QuickNode, Helius)?</b></summary>
<p>No. RADAR is designed to work with public Solana RPC endpoints out-of-the-box. If you already have private RPC credentials, you can configure them locally for enhanced rate limits.</p>
</details>

<details>
<summary><b>Why is Token-2022 inspection critical right now?</b></summary>
<p>Solana Token-2022 extensions allow issuers to set permanent delegates (transferring your tokens without signature) or default account freeze states. Standard DEX frontends often fail to detect these traps until after funds are locked.</p>
</details>

---

## 🛡️ Security & Privacy Guarantees

| Principle | Execution |
| :--- | :--- |
| **Zero Private Keys** | Never asks for, stores, or handles private keys, mnemonic phrases, or signatures. |
| **Strictly Offline Processing** | Client-side DOM parsing. No telemetry tracking, analytics pixels, or external API calls. |
| **Verifiable Bytecode & Slots** | Every finding references exact on-chain slot numbers and instruction types. |
| **Deterministic Checksums** | All standalone release bundles are paired with immutable SHA-256 signatures in [`releases/SHA256SUMS.txt`](releases/SHA256SUMS.txt). |

---

## 🌐 Official Channels & Community

* **🐦 Official X (Twitter)**: [@radraw6o](https://x.com/radraw6o) — Real-time risk alerts & on-chain telemetry
* **🤖 Interactive Telegram Bot**: [@sol_alpha_radar_bot](https://t.me/sol_alpha_radar_bot) — Instant Solana CA risk scanner
* **💬 Research Community Lab**: [t.me/sol_alpha_radar_lab](https://t.me/sol_alpha_radar_lab) — Developer discussions & telemetry feedback
* **📊 Live Liquidity & Chart**: [DexScreener Telemetry](https://dexscreener.com/solana/6a6x3M8xHesyHi5F6zWgCv3CDjRo9NLM3JVNP1LPxbiK)

---

## 📄 License
This public showcase documentation and distribution package is licensed under the [Apache License 2.0](LICENSE).
