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

## License

[MIT](LICENSE).
