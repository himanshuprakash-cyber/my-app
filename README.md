# My App

A Web3 dApp composed with [[N]skills](https://www.nskills.xyz).

## Blueprint: selected nodes

These components were included in this generation:

- **Stylus Rust Contract** — Guide for building Rust smart contracts on Arbitrum Stylus
- **ERC-1155 Stylus Multi-Token** — Deploy and interact with ERC-1155 multi-tokens on Arbitrum Stylus
- **Frontend Scaffold** — Generate a Next.js Web3 application with wagmi, RainbowKit, and smart contract integration
- **Chainlink Price Feed** — Fetch on-chain price feeds from Chainlink Data Feeds on Arbitrum
- **SmartCache Caching** — Enable contract caching for cheaper gas - mycontracts (original) + cached-contracts (with caching)
- **OpenClaw** — Prompt-driven OpenClaw agent block
- **Wallet Authentication** — Wallet connection with RainbowKit and WalletConnect
- **RPC Provider** — Multi-provider RPC configuration with failover for Arbitrum
- **Dune Transaction History** — Fetch transaction history for wallets using Dune Analytics
- **Auditware Analyzer** — Security analysis with Radar for Rust smart contracts

## Project structure

```
my-app/
├── apps/
│   └── web/                    # Next.js app (install dependencies here)
│       ├── src/
│       ├── package.json
│       └── ...
├── contracts/                  # Rust/Stylus smart contracts
│   ├── mycontract/            # Original contract (no caching)
│   │   └── src/lib.rs
│   └── cached-contract/       # Contract with is_cacheable helper
│       └── src/lib.rs
├── docs/                       # Documentation
├── scripts/                     # Deploy / utility scripts (if generated)
├── .gitignore
└── README.md
```

## Quick start

### Prerequisites

- **Node.js** 18+ and **npm** (comes with Node.js)
- **Rust** toolchain and **cargo-stylus** for building/deploying Stylus contracts (see `docs/` and [Stylus SDK](https://github.com/OffchainLabs/stylus-sdk-rs))

### Step-by-step

1. **Clone and enter the project**

   ```bash
   git clone <your-repo-url>
   cd <your-repo-name>
   ```

   ![Clone and enter the project](https://raw.githubusercontent.com/Cradle-app/NSkills/main/apps/web/public/clone-and-enter.png)

2. **Install dependencies** for the Next.js app (this project has no root `package.json`; dependencies live under `apps/web`):

   ```bash
   cd apps/web
   npm install
   ```

   ![Install dependencies](https://raw.githubusercontent.com/Cradle-app/NSkills/main/apps/web/public/install-dep.png)

3. **Environment variables**

   ```bash
   cp .env.example .env
   ```

   Edit `.env` and set:

   - `STYLUS_RPC_URL`: Arbitrum RPC URL for deployment
   - `DEPLOYER_PRIVATE_KEY`: Private key for deployment
   - `PRIVATE_KEY`: Private key for deployment and transactions
   - `NEXT_PUBLIC_WALLETCONNECT_PROJECT_ID`: WalletConnect Cloud project ID for wallet connections
   - `CHAINLINK_FEED_ADDRESS`: Chainlink Data Feed contract address (AggregatorV3Interface)
   - `CHAINLINK_CHAIN`: Chain for Chainlink feed (e.g. ARBITRUM or ARBITRUM_SEPOLIA)
   - `NEXT_PUBLIC_ALCHEMY_API_KEY`: Alchemy API key for RPC access
   - `DUNE_API_KEY`: Dune Analytics API key for blockchain data queries

   ![Environment variables](https://raw.githubusercontent.com/Cradle-app/NSkills/main/apps/web/public/env-var.png)

### Run the web app

```bash
cd apps/web && npm run dev
```

Open [http://localhost:3000](http://localhost:3000).


## Documentation

Check the `docs/` folder for guides that match your blueprint (e.g. frontend setup, contract deployment, API routes).

## License

MIT

---

Generated with [[N]skills](https://www.nskills.xyz)
