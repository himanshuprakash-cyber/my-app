# SmartCache Caching

| Field | Value |
|-------|-------|
| Type | `smartcache-caching` |
| ID | `9f391a03` |
| Category | contracts |
| Tags | cache, gas, optimization, stylus |
| Description | Enable contract caching for cheaper gas |

## Configuration

| Setting | Value |
|---------|-------|
| Crate Version | latest |
| Auto Opt In | Enabled |

## Scripts

| Name | Command |
|------|---------|
| `deploy:sepolia` | `bash scripts/deploy-sepolia.sh` |
| `deploy:mainnet` | `bash scripts/deploy-mainnet.sh` |
| `fix-scripts` | `command -v dos2unix >/dev/null && dos2unix scripts/*.sh 2>/dev/null || echo "Run: dos2unix scripts/*.sh (install with: apt install dos2unix / brew install dos2unix)"` |

## File Structure

This component would generate the following files:

- `contracts/mycontracts/Cargo.toml`
- `contracts/mycontracts/src/lib.rs`
- `contracts/mycontracts/src/main.rs`
- `contracts/mycontracts/rust-toolchain.toml`
- `contracts/mycontracts/.cargo/config.toml`
- `contracts/mycontracts/.gitignore`
- `contracts/mycontracts/.env.example`
- `contracts/cached-contracts/Cargo.toml`
- `contracts/cached-contracts/src/lib.rs`
- `contracts/cached-contracts/src/main.rs`
- `contracts/cached-contracts/rust-toolchain.toml`
- `contracts/cached-contracts/.cargo/config.toml`
- `contracts/cached-contracts/.gitignore`
- `contracts/cached-contracts/.env.example`
- `docs/SMARTCACHE_INTEGRATION.md`
- `scripts/deploy-sepolia.sh`
- `scripts/deploy-mainnet.sh`

## Integration Points

**Depends on:**
- Stylus-rust-contract (`50f955d3`)
- Erc1155-stylus (`da1c9c2e`)

**Provides to:**
- Auditware-analyzing (`1a39118b`)

