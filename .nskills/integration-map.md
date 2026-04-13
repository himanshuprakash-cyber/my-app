# Integration Map

How components connect and what data flows between them.

### Frontend-scaffold --> Openclaw-agent

- **Source**: Frontend-scaffold (`496362a0`)
  - Output ports: App Context (config)
- **Target**: Openclaw-agent (`ff0f1381`)
  - Input ports: Agent Prompt (config)

### Stylus-rust-contract --> Smartcache-caching

- **Source**: Stylus-rust-contract (`50f955d3`)
  - Output ports: Contract Code (contract)
- **Target**: Smartcache-caching (`9f391a03`)
  - Input ports: Contract Input (contract)

### Stylus-rust-contract --> Auditware-analyzing

- **Source**: Stylus-rust-contract (`50f955d3`)
  - Output ports: Contract Code (contract)
- **Target**: Auditware-analyzing (`1a39118b`)
  - Input ports: Contract Input (contract)

### Stylus-rust-contract --> Frontend-scaffold

- **Source**: Stylus-rust-contract (`50f955d3`)
  - Output ports: Contract Code (contract)
- **Target**: Frontend-scaffold (`496362a0`)
  - Input ports: Contract ABI (contract), Network Config (config)

### Smartcache-caching --> Auditware-analyzing

- **Source**: Smartcache-caching (`9f391a03`)
  - Output ports: Cached Contract (contract)
- **Target**: Auditware-analyzing (`1a39118b`)
  - Input ports: Contract Input (contract)

### Frontend-scaffold --> Wallet-auth

- **Source**: Frontend-scaffold (`496362a0`)
  - Output ports: App Context (config)
- **Target**: Wallet-auth (`b2d95739`)
  

### Frontend-scaffold --> Rpc-provider

- **Source**: Frontend-scaffold (`496362a0`)
  - Output ports: App Context (config)
- **Target**: Rpc-provider (`56fc9cc9`)
  

### Frontend-scaffold --> Dune-transaction-history

- **Source**: Frontend-scaffold (`496362a0`)
  - Output ports: App Context (config)
- **Target**: Dune-transaction-history (`f2e39b98`)
  

### Stylus-rust-contract --> Chainlink-price-feed

- **Source**: Stylus-rust-contract (`50f955d3`)
  - Output ports: Contract Code (contract)
- **Target**: Chainlink-price-feed (`a777ff22`)
  

### Erc1155-stylus --> Smartcache-caching

- **Source**: Erc1155-stylus (`da1c9c2e`)
  - Output ports: Multi-Token Contract (contract)
- **Target**: Smartcache-caching (`9f391a03`)
  - Input ports: Contract Input (contract)
