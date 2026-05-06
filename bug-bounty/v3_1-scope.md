# Gearbox V3 scope

Generally, we care about security of the whole codebase, including contracts that are not deployed yet, so the bug bounty program scope is the following:

- Governance: [permissionless@48a7273a](https://github.com/Gearbox-protocol/permissionless/tree/48a7273a8b1c58690fc9761d01c8a6701bffd6f3) (everything in `contracts/` except `contracts/test/`)
- Core: [core-v3@b038597d](https://github.com/Gearbox-protocol/core-v3/tree/b038597d9070d9fd18593a6ae9c3d28ca931bb73) (everything in `contracts/` except `contracts/test/`)
- Oracles: [oracles-v3@287739a0](https://github.com/Gearbox-protocol/oracles-v3/tree/287739a0d85d4c1a2ad15b8aebcc2fcb4db0af4d) (everything in `contracts/` except `contracts/test/`)
- Integrations: [integrations-v3@8c4cf2ac](https://github.com/Gearbox-protocol/integrations-v3/tree/8c4cf2ac8e9a4a5b49ffd955358e55fd5401605c) (everything in `contracts/` except `contracts/test/`)

## Deployed contracts

This is the list of contracts deployed on Ethereum Mainnet that can be used for PoC.
Unless specified otherwise, all relevant deployed contracts have the `version` constant set between `3_10` and `3_20` (non-inclusive).

There are two sources that can help with discovery:
- [AddressProviderV3](https://etherscan.io/address/0xF7f0a609BfAb9a0A98786951ef10e5FE26cC1E38#readContract) - this contract contains important system-wide addresses.
- [Bytecode Repository Portal](https://permissionless.gearbox.foundation/bytecode) - this portal contains lists all audited contract types used by Gearbox, as well as the latest source and the list of deployed contracts for each type. 
All contracts that are at least somewhat relevant for on-chain operations are deployed from the Bytecode Repository, with exception of some contracts that can be found in AddressProviderV3.
