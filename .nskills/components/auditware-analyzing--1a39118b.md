# Auditware Analyzer

| Field | Value |
|-------|-------|
| Type | `auditware-analyzing` |
| ID | `1a39118b` |
| Category | contracts |
| Tags | security, audit, analysis, stylus |
| Description | Security analysis with Radar |

## Configuration

| Setting | Value |
|---------|-------|
| Output Format | both |
| Severity Filter | low, medium, high |
| Project Path | . |

## Scripts

| Name | Command |
|------|---------|
| `security:install` | `bash scripts/install-radar.sh` |
| `security:analyze` | `bash scripts/run-radar.sh` |
| `deploy:sepolia` | `bash scripts/deploy-sepolia.sh` |
| `deploy:mainnet` | `bash scripts/deploy-mainnet.sh` |
| `fix-scripts` | `command -v dos2unix >/dev/null && dos2unix scripts/*.sh 2>/dev/null || echo "Run: dos2unix scripts/*.sh (install: apt install dos2unix / brew install dos2unix)"` |

## File Structure

This component would generate the following files:

- `docs/RADAR_SECURITY_ANALYSIS.md`
- `scripts/install-radar.sh`
- `scripts/run-radar.sh`
- `scripts/deploy-sepolia.sh`
- `scripts/deploy-mainnet.sh`

## Integration Points

**Depends on:**
- Stylus-rust-contract (`50f955d3`)
- Smartcache-caching (`9f391a03`)

