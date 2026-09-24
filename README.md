# RPC Hub

> EVM RPC Chain Explorer — Discover, test, and monitor RPC endpoints across 500+ EVM-compatible blockchains.

🌐 [rpchub.top](https://rpchub.top)

---

## What is RPC Hub?

RPC Hub is a Web3 infrastructure discovery and verification platform. It solves a fundamental pain point for blockchain developers: **finding reliable RPC endpoints and knowing which ones actually work well right now.**

[Chainlist](https://chainlist.org) only tells you whether an RPC is reachable from your browser — with CORS limitations causing many false offline reports. RPC Hub performs **server-side probing** to give you accurate, real-time latency and availability data.

| Pain Point | RPC Hub Solution |
|---|---|
| Chainlist only checks reachability, not performance | Real-time latency, block height verification, and availability rates |
| Browser detection has CORS false positives | Server-side probing with zero CORS restrictions |
| Infura / Alchemy / QuickNode each in their own silo | One dashboard to compare all providers + self-hosted nodes |
| RPC outages go unnoticed until users complain | 7×24 monitoring with multi-channel alerts |
| No built-in debugging tools | JSON-RPC Playground + Cast Terminal in the browser |

---

## Features

### 🔗 Chain Explorer

- **500+ EVM chains** with full metadata (chain ID, native currency, explorers, faucets)
- **Real-time RPC status** — latency, online/offline, block height for every endpoint
- **One-click wallet integration** — add any network to MetaMask or other wallets
- **Search & filter** by chain name, chain ID, or RPC URL
- Data source: [chainlist.org/rpcs.json](https://chainlist.org/rpcs.json)

### 🛠 JSON-RPC Playground

- Send raw JSON-RPC requests directly from the browser via server-side proxy
- Method presets for common calls (`eth_blockNumber`, `eth_getBalance`, `eth_call`, etc.)
- Request history saved locally
- Export requests as cURL commands

### 🖥 Cast Terminal

- Web-based terminal for [Foundry's cast](https://book.getfoundry.sh/cast/) CLI
- Execute read-only commands: `cast block-number`, `cast balance`, `cast call`, etc.
- Safety restrictions prevent dangerous operations (`cast send`, `cast wallet`)

---

## How It Differs from Chainlist

| Dimension | Chainlist | RPC Hub |
|---|---|---|
| Detection Method | Browser frontend fetch | Server-side multi-node probing |
| CORS Limitations | Yes — many false offline reports | None |
| Latency Data | None | Real-time global latency across regions |
| Historical Data | None | Complete time-series data |
| Alerting | None | Multi-channel push notifications |

---

## Target Users

| User | Core Need |
|---|---|
| Web3 Independent Developers | Find free/affordable reliable RPCs |
| DeFi Protocol Teams | Multi-RPC failover, on-chain data verification |
| MEV Searchers / Trading Bots | Low-latency RPC selection |
| NFT Projects | RPC stability during high-traffic mints |
| Exchanges / Custodians | Node sync status monitoring |

---

## License

MIT
