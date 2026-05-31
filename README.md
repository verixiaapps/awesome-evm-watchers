# Awesome EVM watchers

Tools, dashboards, and public datasets that *watch* EVM chains rather than write to them. Read-only observability for transfers, prices, MEV, governance, and on-chain reputation.

Excludes wallets, dexes, and aggregators (those are not watchers).

## Tools

### Transfer & balance watchers

- [whale-watcher](https://github.com/asuranwhale/whale-watcher) - CLI/lib that streams ERC20 transfers above a threshold. Zero deps.
- [eth-events](https://github.com/topics/eth-events) - Various community ERC20/event-watching scripts.
- [tenderly-alerts](https://docs.tenderly.co/alerts) - Hosted contract event alerts.

### Mempool watchers

- [Blocknative Mempool](https://www.blocknative.com/explorer) - Hosted real-time mempool with WebSockets.
- [Flashbots dashboard](https://www.flashbots.net/) - MEV-Boost relay stats and protect data.

### Gas watchers

- [Etherscan Gas Tracker](https://etherscan.io/gastracker) - The reference.
- [ETH Gas Station](https://ethgasstation.info/) - Long-running historical view.
- [Blocknative Gas API](https://www.blocknative.com/gas-platform) - JSON gas estimates with confidence intervals.

### Price watchers

- [Chainlink Data Feeds](https://data.chain.link/) - On-chain oracle reference for production code.
- [Pyth](https://pyth.network/) - Pull-style oracle, alternative to Chainlink.
- [API3](https://api3.org/) - First-party data feeds.

### Governance watchers

- [Tally](https://www.tally.xyz/) - DAO governance dashboard, multi-chain.
- [Snapshot](https://snapshot.org/) - Off-chain voting; useful as a watcher even if not on-chain.

## Datasets

- [Etherscan Verified Contracts](https://etherscan.io/contractsVerified) - Source-verified contracts; good for filtering noise.
- [Token Lists](https://tokenlists.org/) - Community token registries; canonical decimals/symbol per address.
- [The Graph hosted subgraphs](https://thegraph.com/) - Many chains have community subgraphs for ERC20/721/1155 events.

## Standards & references

- [ERC-20](https://eips.ethereum.org/EIPS/eip-20) - The token standard. The `Transfer(address,address,uint256)` event is the most-watched signal in crypto.
- [ERC-721](https://eips.ethereum.org/EIPS/eip-721) - NFT transfers (also a `Transfer` event but with `tokenId` indexed).
- [ERC-1155](https://eips.ethereum.org/EIPS/eip-1155) - Multi-token transfers (`TransferSingle`/`TransferBatch`).
- [JSON-RPC spec](https://ethereum.org/en/developers/docs/apis/json-rpc/) - Authoritative reference for `eth_getLogs` filter shape.

## Self-hosted options

- [Erigon](https://github.com/erigontech/erigon) - Performant full node; good for indexing.
- [Reth](https://github.com/paradigmxyz/reth) - Modular Rust client; growing watcher ecosystem.
- [Substreams](https://substreams.streamingfast.io/) - Streaming-first indexing primitives.

## Contributing

PRs welcome. Each entry must:

1. Be open source, free, or be an authoritative reference.
2. Specifically observe (not write to) EVM chain state.
3. Be currently maintained.

## License

[MIT](LICENSE).
