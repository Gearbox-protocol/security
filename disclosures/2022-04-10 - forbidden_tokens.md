# Vulnerability disclosure 2022-04-10

## Summary

- A vulnerability was reported by a @0xmikko
- No funds are at risk
- No need to any actions in current system parameters



## Details of vulnerability

- (CreditFilter.sol)[https://github.com/Gearbox-protocol/gearbox-contracts/blob/master/contracts/credit/CreditFilter.sol] contracts have forbidToken interface
- If token is forbidden and price of chainlink oracle higher than real market price, attacker can open credit account, send forbidden tokens directly to credit account and then increase borrow amount
- due to incorrect work of fastcheck for this case, it is possible to drain funds from credit account by trading on whitelisted DEXes and sandwich-ing this trades


## Details of fix
1. If token is forbidden and chainlink price is incorrect, it's liquidation threshold should be changed to 0 
2. If pp. 1 doesn't possible to do quickly, credit managers should be paused


## Timeline of events

- **Apr 10, 2022, 07:10 pm UTC** @0xmirro informed about possible attack in the case of forbidding token
- **Apr 10, 2022, 08:16 pm UTC** Gearbox members checked current protocol parameters to be sure no funds at risk

