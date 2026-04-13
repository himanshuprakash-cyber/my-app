# Architecture

## Dependency Graph

```mermaid
graph TD
  50f955d3["Stylus-rust-contract (stylus-rust-contract)"]
  da1c9c2e["Erc1155-stylus (erc1155-stylus)"]
  496362a0["Frontend-scaffold (frontend-scaffold)"]
  a777ff22["Chainlink-price-feed (chainlink-price-feed)"]
  9f391a03["Smartcache-caching (smartcache-caching)"]
  ff0f1381["Openclaw-agent (openclaw-agent)"]
  b2d95739["Wallet-auth (wallet-auth)"]
  56fc9cc9["Rpc-provider (rpc-provider)"]
  f2e39b98["Dune-transaction-history (dune-transaction-history)"]
  1a39118b["Auditware-analyzing (auditware-analyzing)"]
  496362a0 --> ff0f1381
  50f955d3 --> 9f391a03
  50f955d3 --> 1a39118b
  50f955d3 --> 496362a0
  9f391a03 --> 1a39118b
  496362a0 --> b2d95739
  496362a0 --> 56fc9cc9
  496362a0 --> f2e39b98
  50f955d3 --> a777ff22
  da1c9c2e --> 9f391a03
```

## Execution / Implementation Order

1. **Stylus-rust-contract** (`50f955d3`)
2. **Erc1155-stylus** (`da1c9c2e`)
3. **Frontend-scaffold** (`496362a0`)
4. **Chainlink-price-feed** (`a777ff22`)
5. **Smartcache-caching** (`9f391a03`)
6. **Openclaw-agent** (`ff0f1381`)
7. **Wallet-auth** (`b2d95739`)
8. **Rpc-provider** (`56fc9cc9`)
9. **Dune-transaction-history** (`f2e39b98`)
10. **Auditware-analyzing** (`1a39118b`)
