# Scripts

| Name | Command | Description |
|------|---------|-------------|
| `deploy:multitoken` | `ts-node scripts/deploy-erc1155.ts` | Deploy ERC1155 multi-token |
| `multitoken:info` | `ts-node scripts/multitoken-info.ts` | Get multi-token information |
| `dev` | `next dev` | Start development server |
| `build` | `next build` | Build for production |
| `start` | `next start` | Start production server |
| `lint` | `next lint` | Run ESLint |
| `deploy:sepolia` | `bash scripts/deploy-sepolia.sh` |  |
| `deploy:mainnet` | `bash scripts/deploy-mainnet.sh` |  |
| `fix-scripts` | `command -v dos2unix >/dev/null && dos2unix scripts/*.sh 2>/dev/null || echo "Run: dos2unix scripts/*.sh (install with: apt install dos2unix / brew install dos2unix)"` |  |
| `wallet:setup` | `echo "Get your WalletConnect Project ID from https://dashboard.reown.com"` | Instructions for wallet setup |
| `rpc:health` | `tsx src/lib/rpc/health-check.ts` |  |
| `security:install` | `bash scripts/install-radar.sh` |  |
| `security:analyze` | `bash scripts/run-radar.sh` |  |
| `deploy:sepolia` | `bash scripts/deploy-sepolia.sh` |  |
| `deploy:mainnet` | `bash scripts/deploy-mainnet.sh` |  |
| `fix-scripts` | `command -v dos2unix >/dev/null && dos2unix scripts/*.sh 2>/dev/null || echo "Run: dos2unix scripts/*.sh (install: apt install dos2unix / brew install dos2unix)"` |  |
