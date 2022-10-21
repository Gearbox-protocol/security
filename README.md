# Gearbox protocol

Gearbox is a generalized leverage protocol: it allows you to take leverage in one place and then use it across various
DeFi protocols and platforms in a composable way. The protocol has two sides to it: passive liquidity providers who earn higher APY
by providing liquidity; active traders, farmers, or even other protocols who can borrow those assets to trade or farm with x4+ leverage.

## Repository overview

This repository contains audit reports and incident disclosures for Gearbox protocol:

- `audits` contains final reports submitted by security audit teams. Reports dated before 2022 are mainly relevant for Gearbox V1, although some deployed core contracts from V1 (such as `ACL.sol` or `AddressProvider.sol`) are used in V2. Reports dated after 2022 detail findings for Gearbox V2.
- `disclosures` contains reports made by the Gearbox team regarding discovered vulnerabilities and other security incidents, as well as means deployed to address them.
