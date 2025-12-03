
   # BlackTrace Protocol

  **Cross-chain settlement without the bridge.**

  Bridges get hacked. Over $2 billion lost. BlackTrace uses hash-locked escrows instead - your assets stay on their native chains, locked by
  cryptography, not custody.

  ## What is BlackTrace?

  BlackTrace is a trustless cross-chain atomic settlement protocol. It enables large OTC trades between parties who don't trust each other, without
  counterparty risk, front-running, or intermediaries.

  **How it works:**

  1. Alice locks assets on Chain A with a secret key
  2. Bob locks assets on Chain B with the same key
  3. Alice claims from Chain B by revealing the secret
  4. Bob uses the revealed secret to claim from Chain A

  *Currently supports: SOL-ZEC (Solana ↔ Zcash) and STRK-ZEC (Starknet ↔ Zcash)*

  **Both get paid, or both get refunded. No bridge. No custody.**

  ## Repository

  | Repository | Description |
  |------------|-------------|
  | [blacktrace](https://github.com/blacktrace-protocol/blacktrace) | Core protocol implementation (Go, Rust, TypeScript) |

  ## Quick Links

  ### Website
  - [blacktrace.xyz](https://blacktrace.xyz)

  ### Vision
  - [The Quest for Bridgeless Settlement](https://github.com/blacktrace-protocol/blacktrace/blob/main/docs/vision/quest-for-bridgeless-settlement.md) -
   Why BlackTrace exists

  ### Getting Started
  - [Quickstart Guide](https://github.com/blacktrace-protocol/blacktrace/blob/main/docs/QUICKSTART.md) - Run BlackTrace in 5 minutes
  - [Architecture](https://github.com/blacktrace-protocol/blacktrace/blob/main/docs/ARCHITECTURE.md) - System design

  ### For Developers (Roadmap)
  - [Developer Vision](https://github.com/blacktrace-protocol/blacktrace/blob/main/docs/vision/developer-vision.md) - PEXes and the future
  - [API Reference](https://github.com/blacktrace-protocol/blacktrace/blob/main/docs/API.md) - Complete endpoint docs
  - [Adding New Chains](https://github.com/blacktrace-protocol/blacktrace/blob/main/docs/reference/CHAIN_CONNECTORS.md) - Extend to other blockchains

  ## Technology

  - **P2P Network**: libp2p with encrypted gossipsub
  - **Encryption**: ECIES (P-256) for private negotiation
  - **Settlement**: HTLC atomic swaps with HASH160 for cross-chain compatibility
  - **Chains**: Zcash, Solana, Starknet

  ## Working Demos

  | Demo | Chains | Status |
  |------|--------|--------|
  | SOL-ZEC | Solana ↔ Zcash | ✅ Live |
  | STRK-ZEC | Starknet ↔ Zcash | ✅ Live |

  ## Use Cases

  - **DAO Treasuries** - Trustless diversification with on-chain audit trails
  - **Privacy Whales** - No KYC, no desk seeing your positions
  - **Cross-border Trades** - No legal framework needed
  - **OTC Platforms** - Build Binance OTC without custody risk

  ## License

  MIT


