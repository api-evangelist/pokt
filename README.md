# Pocket Network (POKT)

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

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
