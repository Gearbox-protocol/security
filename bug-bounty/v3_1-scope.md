# Gearbox V3.1 scope

Generally, we care about security of the whole codebase, including contracts that are not deployed yet, so the bug bounty program scope is the following:

- Permissionless: [permissionless](https://github.com/Gearbox-protocol/permissionless) (everything in `contracts/` except `contracts/test/`)
- Core: [core-v3](https://github.com/Gearbox-protocol/core-v3) (everything in `contracts/` except `contracts/test/`)
- Oracles: [oracles-v3](https://github.com/Gearbox-protocol/oracles-v3) (everything in `contracts/` except `contracts/test/`)
- Integrations: [integrations-v3](https://github.com/Gearbox-protocol/integrations-v3) (everything in `contracts/` except `contracts/test/`)
- Bots: [bots-v3](https://github.com/Gearbox-protocol/bots-v3) (everything in `contracts/bots`)
- Periphery: [periphery-v3](https://github.com/Gearbox-protocol/periphery-v3) (everything in `contracts/emergency`, `contracts/kyc` and `contracts/migration`, except contracts with `*Previewer` in name)

For repositories above, only the `main` or `master` branch is considered within scope, unless specified otherwise.

## Deployed contracts

This is the list of contracts deployed on Ethereum Mainnet that can be used for PoC.
Unless specified otherwise, all relevant deployed contracts have the `version` constant set between `3_10` and `3_20` (non-inclusive).

There are two sources that can help with discovery:
- [AddressProviderV3](https://etherscan.io/address/0xF7f0a609BfAb9a0A98786951ef10e5FE26cC1E38#readContract) - this contract contains important system-wide addresses.
- [Bytecode Repository Portal](https://permissionless.gearbox.foundation/bytecode) - this portal contains lists all audited contract types used by Gearbox, as well as the latest source and the list of deployed contracts for each type. 
All contracts that are at least somewhat relevant for on-chain operations are deployed from the Bytecode Repository, with exception of some contracts that can be found in AddressProviderV3.
