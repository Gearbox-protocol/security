# Gearbox protocol

Gearbox is a generalized leverage protocol. It has two sides to it: passive liquidity providers who earn low-risk APY by providing single-asset liquidity; and active farmers, firms, or even other protocols who borrow those assets to trade or farm with even x10 leverage.

Gearbox Protocol allows anyone to take DeFi-native leverage and then use it across various (DeFi & more) protocols in a composable way. You take leverage with Gearbox and then use it on other protocols you already love: Uniswap, Curve, Convex, Lido, etc. For example, you can leverage trade on Uniswap, leverage farm on Yearn, make delta-neutral strategies, get Leverage-as-a-Service for your structured product, and more... Thanks to the Credit Accounts primitive! 

_Some compare composable leverage as a primitive to DeFi-native prime brokerage._


## Repository overview

This repository contains audit reports and incident disclosures for Gearbox protocol:

- `audits` contains final reports submitted by security audit teams. Reports dated before 2022 are mainly relevant for Gearbox V1, although some deployed core contracts from V1 (such as `ACL.sol` or `AddressProvider.sol`) are used in V2. Reports dated after 2022 detail findings for Gearbox V2.
- `disclosures` contains reports made by the Gearbox team regarding discovered vulnerabilities and other security incidents, as well as means deployed to address them.
