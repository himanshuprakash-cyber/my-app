# Environment Variables

| Key | Description | Required | Secret | Default |
|-----|-------------|----------|--------|---------|
| `STYLUS_RPC_URL` | Arbitrum RPC URL for deployment | Yes | No | https://sepolia-rollup.arbitrum.io/rpc |
| `DEPLOYER_PRIVATE_KEY` | Private key for deployment | Yes | Yes |  |
| `NEXT_PUBLIC_ERC1155_ADDRESS` | Deployed ERC1155 multi-token address | No | No |  |
| `PRIVATE_KEY` | Private key for deployment and transactions | Yes | Yes |  |
| `ERC1155_DEPLOYMENT_API_URL` | URL of the ERC1155 deployment API | No | No | http://localhost:4002 |
| `NEXT_PUBLIC_WALLETCONNECT_PROJECT_ID` | WalletConnect Cloud project ID for wallet connections | Yes | No |  |
| `NEXT_PUBLIC_APP_NAME` | Application name displayed in wallet dialogs | No | No | My DApp |
| `CHAINLINK_FEED_ADDRESS` | Chainlink Data Feed contract address (AggregatorV3Interface) | Yes | No | 0x639Fe6ab55C921f74e7fac1ee960C0B6293ba612 |
| `CHAINLINK_CHAIN` | Chain for Chainlink feed (e.g. ARBITRUM or ARBITRUM_SEPOLIA) | Yes | No | ARBITRUM |
| `NEXT_PUBLIC_ALCHEMY_API_KEY` | Alchemy API key for RPC access | Yes | No |  |
| `DUNE_API_KEY` | Dune Analytics API key for blockchain data queries | Yes | Yes |  |
