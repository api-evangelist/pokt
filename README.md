# Pocket Network (POKT)

Pocket Network is a decentralized, permissionless RPC infrastructure network providing free public API access to 60+ blockchain chains including Ethereum, Avalanche, Polygon, Solana, Base, Arbitrum, Optimism, and other EVM-compatible and non-EVM networks. The Shannon upgrade (June 2025) made Pocket the first open, permissionless API network where anyone can stake POKT tokens to deploy gateways and supply relay nodes without centralized approval.

## APIs

- **Public RPC API** - Free, keyless JSON-RPC 2.0 endpoints for 60+ chains via `https://{chain}.api.pocket.network`
- **Shannon Chain API** - Cosmos SDK REST, gRPC, and CometBFT RPC for protocol-level interactions
- **PATH Gateway API** - Open-source gateway framework health, readiness, and metrics endpoints

## Resources

- [Website](https://pocket.network/)
- [Documentation](https://docs.pocket.network/)
- [Public API Portal](https://api.pocket.network/)
- [GitHub Organization](https://github.com/pokt-network/)
- [Forum](https://forum.pokt.network/)
- [Explorer](https://explorer.pokt.network/)
- [Blog](https://pocket.network/blog/)
- [Discord](https://discord.gg/pokt)

## Access

All public RPC endpoints follow the pattern:

```
POST https://{chain-slug}.api.pocket.network
Content-Type: application/json
```

No API key required. Example chains: `eth`, `poly`, `avax`, `base`, `arb-one`, `op`, `solana`.

## Plans & Pricing

See [plans/plans.yml](plans/plans.yml) for full tier details.

| Plan | Cost | Rate Limit |
|------|------|------------|
| Public RPC (Free) | $0 | 2000 req/min per IP |
| Application Staking | POKT stake | Unlimited |
| Gateway Delegation | Varies by operator | Unlimited |
| PATH Operator (Wholesale) | ~$1.58/M ETH relays | Unlimited |

## FinOps

Pricing is based on Compute Units (CUs) per relay. See [finops/finops.yml](finops/finops.yml) for chain-specific CU rates and volume rebate tiers (up to 40% discount at 1.25T CU/day).

## Catalog

This repository is part of the [APIs.json](https://apisjson.org) catalog maintained by [API Evangelist](https://apievangelist.com).
