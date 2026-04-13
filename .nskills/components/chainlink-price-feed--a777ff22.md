# Chainlink Price Feed

| Field | Value |
|-------|-------|
| Type | `chainlink-price-feed` |
| ID | `a777ff22` |
| Category | protocols |
| Tags | chainlink, oracle, prices, feeds, arbitrum, aggregator |
| Description | On-chain price feeds from Chainlink Data Feeds |

## Configuration

| Setting | Value |
|---------|-------|
| Chain | arbitrum |
| Feed Address | 0x639Fe6ab55C921f74e7fac1ee960C0B6293ba612 |

## Environment Variables

| Key | Description | Required | Secret | Default |
|-----|-------------|----------|--------|---------|
| `CHAINLINK_FEED_ADDRESS` | Chainlink Data Feed contract address (AggregatorV3Interface) | Yes | No | 0x639Fe6ab55C921f74e7fac1ee960C0B6293ba612 |
| `CHAINLINK_CHAIN` | Chain for Chainlink feed (e.g. ARBITRUM or ARBITRUM_SEPOLIA) | Yes | No | ARBITRUM |

## File Structure

This component would generate the following files:

- `chainlink-price-feed.md` (docs)

## Integration Points

**Depends on:**
- Stylus-rust-contract (`50f955d3`)

