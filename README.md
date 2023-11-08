# Gearbox Protocol

Gearbox Protocol brings you **onchain credit**, allowing anyone to margin trade on Uniswap, leverage farm on Curve, leverage stake on Lido, and use 10X more capital on many DeFi protocols you love, as well as RWA & NFTs. Making decentralized leverage a reality thanks to Credit Account abstraction! 

_[See the blog post for more information on V3 and new features.](https://blog.gearbox.fi/gearbox-protocol-v3-the-onchain-credit-layer/)_

Gearbox Protocol uses Credit Account abstraction to bring together lending and prime brokerage in the same protocol. Lenders deposit assets to earn passive yield, while the composable leverage side users borrow these assets to create spot leverage positions, which can be used across DeFi. That could be margin trading on Uniswap, farming on Curve and Balancer, leverage staking on Lido and Rocketpool, and a lot more. All of that is made possible with Gearbox’s innovative Credit Account abstraction, creating the base layer of DeFi leverage.

Information on bug bounty and audits can be found in the [general docs](https://docs.gearbox.finance/risk-and-security/audits-bug-bounty).

## Repository overview

This repository contains audit reports and incident disclosures for Gearbox Protocol:

- `audits` contains final reports submitted by security audit teams. Reports dated before 2022 are mainly relevant for Gearbox V1, although some deployed core contracts from V1 (such as `ACL.sol` or `AddressProvider.sol`) are used in V2. Reports dated after 2022 detail findings for Gearbox V2, up to autumn 2023. **Reports from autumn 2023 are relevant for V3 directly.**
- 
- `disclosures` contains reports made by the Gearbox devleopers regarding discovered vulnerabilities and other security incidents after being confirmed and fixed, as well as means deployed to address them.
