# Gearbox V2 scope

Gearbox V2 codebase is generally split across the following two repositories:

- Core: [core-v2@98a984d](https://github.com/Gearbox-protocol/core-v2/tree/98a984d37fa590e89ff976fe9e2a523b217d50ef)
- Integrations: [integrations-v3@02f239f](https://github.com/Gearbox-protocol/integrations-v3/tree/02f239fee250fb11b16a28974e71e73264de50b2)

You may however notice that deployed contracts sometimes don't match those listed above: some of them (like `AccountFactory` or most `PoolService` contracts) stayed from V1, while others (like `LinearInterestRateModelV3`) were ported from V3.

To remove potential confusion, the bug bounty program is limited only to deployed contracts from the list below, and findings of Critical or High severity.

## Deployed contracts

### Core

- `ACL`
  - [`0x523dA3a8961E4dD4f6206DBf7E6c749f51796bb3`](https://etherscan.io/address/0x523dA3a8961E4dD4f6206DBf7E6c749f51796bb3)
- `AccountFactory`
  - [`0x444CD42BaEdDEB707eeD823f7177b9ABcC779C04`](https://etherscan.io/address/0x444CD42BaEdDEB707eeD823f7177b9ABcC779C04)
- `AddressProvider`
  - [`0xcF64698AFF7E5f27A11dff868AF228653ba53be0`](https://etherscan.io/address/0xcF64698AFF7E5f27A11dff868AF228653ba53be0)
- `BlacklistHelper`
  - [`0xFfbF344741654a1B9Ab1286Cf05A42f275F67839`](https://etherscan.io/address/0xFfbF344741654a1B9Ab1286Cf05A42f275F67839)
- `ContractsRegister`
  - [`0xA50d4E7D8946a7c90652339CDBd262c375d54D99`](https://etherscan.io/address/0xA50d4E7D8946a7c90652339CDBd262c375d54D99)
- `CreditConfigurator`
  - [`0x28b1d625ef7F35afdC35F2B1f4143CCf8EFD375F`](https://etherscan.io/address/0x28b1d625ef7F35afdC35F2B1f4143CCf8EFD375F)
  - [`0x403404eEFd0D0C9E9268DA80A5ba08A02E23FFB7`](https://etherscan.io/address/0x403404eEFd0D0C9E9268DA80A5ba08A02E23FFB7)
  - [`0xea3B73341a91e5c661Cbd54CF80DB3458Ff05c6f`](https://etherscan.io/address/0xea3B73341a91e5c661Cbd54CF80DB3458Ff05c6f)
  - [`0x0E963037B755761F5174A72516c6234c20cD9b98`](https://etherscan.io/address/0x0E963037B755761F5174A72516c6234c20cD9b98)
  - [`0xa68FE321838b6d2fD64feD8A2C5Ec5B9Ff3a348e`](https://etherscan.io/address/0xa68FE321838b6d2fD64feD8A2C5Ec5B9Ff3a348e)
  - [`0x19e29A2fb9b442D2a6C371121A4Ad009794bE3a0`](https://etherscan.io/address/0x19e29A2fb9b442D2a6C371121A4Ad009794bE3a0)
  - [`0xcc000017BeEDCBc7fAb3e57FAB3Cb72c2D00a343`](https://etherscan.io/address/0xcc000017BeEDCBc7fAb3e57FAB3Cb72c2D00a343)
- `CreditFacade`
  - [`0x5BcB06c56e8F28da0b038a373199240ca3F5a2f4`](https://etherscan.io/address/0x5BcB06c56e8F28da0b038a373199240ca3F5a2f4) 
  - [`0x34EE4eed88BCd2B5cDC3eF9A9DD0582EE538E541`](https://etherscan.io/address/0x34EE4eed88BCd2B5cDC3eF9A9DD0582EE538E541)
  - [`0xc9E3453E212A13169AaA66aa39DCcE82aE6966B7`](https://etherscan.io/address/0xc9E3453E212A13169AaA66aa39DCcE82aE6966B7)
  - [`0xB36466F0c3F34aB1f029b7Df798F395f97Eb4BcF`](https://etherscan.io/address/0xB36466F0c3F34aB1f029b7Df798F395f97Eb4BcF)
  - [`0x013A9C05Be13D802f3d682bB5F5DF03Be485e3b6`](https://etherscan.io/address/0x013A9C05Be13D802f3d682bB5F5DF03Be485e3b6)
  - [`0x14C3e68b87eEEc5D6Ba21c85D467E4f7f961759c`](https://etherscan.io/address/0x14C3e68b87eEEc5D6Ba21c85D467E4f7f961759c)
  - [`0x8051699299F929a55F74b550CDB2d9c15C023A87`](https://etherscan.io/address/0x8051699299F929a55F74b550CDB2d9c15C023A87)
- `CreditManager`
  - [`0x672461Bfc20DD783444a830Ad4c38b345aB6E2f7`](https://etherscan.io/address/0x672461Bfc20DD783444a830Ad4c38b345aB6E2f7)
  - [`0x95357303f995e184A7998dA6C6eA35cC728A1900`](https://etherscan.io/address/0x95357303f995e184A7998dA6C6eA35cC728A1900)
  - [`0x5887ad4Cb2352E7F01527035fAa3AE0Ef2cE2b9B`](https://etherscan.io/address/0x5887ad4Cb2352E7F01527035fAa3AE0Ef2cE2b9B)
  - [`0xe0bCE4460795281d39c91da9B0275BcA968293de`](https://etherscan.io/address/0xe0bCE4460795281d39c91da9B0275BcA968293de)
  - [`0xc62BF8a7889AdF1c5Dc4665486c7683ae6E74e0F`](https://etherscan.io/address/0xc62BF8a7889AdF1c5Dc4665486c7683ae6E74e0F)
  - [`0xA3E1e0d58FE8dD8C9dd48204699a1178f1B274D8`](https://etherscan.io/address/0xA3E1e0d58FE8dD8C9dd48204699a1178f1B274D8)
  - [`0x4C6309fe2085EfE7A0Cfb426C16Ef3b41198cCE3`](https://etherscan.io/address/0x4C6309fe2085EfE7A0Cfb426C16Ef3b41198cCE3)
- `DegenNFT`
  - [`0xB829a5b349b01fc71aFE46E50dD6Ec0222A6E599`](https://etherscan.io/address/0xB829a5b349b01fc71aFE46E50dD6Ec0222A6E599)
- `GearToken`
  - [`0xBa3335588D9403515223F109EdC4eB7269a9Ab5D`](https://etherscan.io/address/0xBa3335588D9403515223F109EdC4eB7269a9Ab5D)
- `DieselToken`
  - [`0x6CFaF95457d7688022FC53e7AbE052ef8DFBbdBA`](https://etherscan.io/address/0x6CFaF95457d7688022FC53e7AbE052ef8DFBbdBA)
  - [`0xc411dB5f5Eb3f7d552F9B8454B2D74097ccdE6E3`](https://etherscan.io/address/0xc411dB5f5Eb3f7d552F9B8454B2D74097ccdE6E3)
  - [`0xF21fc650C1B34eb0FDE786D52d23dA99Db3D6278`](https://etherscan.io/address/0xF21fc650C1B34eb0FDE786D52d23dA99Db3D6278)
  - [`0xe753260F1955e8678DCeA8887759e07aa57E8c54`](https://etherscan.io/address/0xe753260F1955e8678DCeA8887759e07aa57E8c54)
  - [`0x2158034dB06f06dcB9A786D2F1F8c38781bA779d`](https://etherscan.io/address/0x2158034dB06f06dcB9A786D2F1F8c38781bA779d)
  - [`0x8A1112AFef7F4FC7c066a77AABBc01b3Fff31D47`](https://etherscan.io/address/0x8A1112AFef7F4FC7c066a77AABBc01b3Fff31D47)
- `LinearInterestRateModelV3`
  - [`0x5a08D449322c1B4777F7b0cd878A485cC8761fe9`](https://etherscan.io/address/0x5a08D449322c1B4777F7b0cd878A485cC8761fe9)
  - [`0xF0966D9094334Fee8e423C49628D9d06343aF06f`](https://etherscan.io/address/0xF0966D9094334Fee8e423C49628D9d06343aF06f)
- `PoolService`
  - [`0x24946bCbBd028D5ABb62ad9B635EB1b1a67AF668`](https://etherscan.io/address/0x24946bCbBd028D5ABb62ad9B635EB1b1a67AF668)
  - [`0x86130bDD69143D8a4E5fc50bf4323D48049E98E4`](https://etherscan.io/address/0x86130bDD69143D8a4E5fc50bf4323D48049E98E4)
  - [`0xB03670c20F87f2169A7c4eBE35746007e9575901`](https://etherscan.io/address/0xB03670c20F87f2169A7c4eBE35746007e9575901)
  - [`0xB2A015c71c17bCAC6af36645DEad8c572bA08A08`](https://etherscan.io/address/0xB2A015c71c17bCAC6af36645DEad8c572bA08A08)
  - [`0xB8cf3Ed326bB0E51454361Fb37E9E8df6DC5C286`](https://etherscan.io/address/0xB8cf3Ed326bB0E51454361Fb37E9E8df6DC5C286)
  - [`0x79012c8d491DcF3A30Db20d1f449b14CAF01da6C`](https://etherscan.io/address/0x79012c8d491DcF3A30Db20d1f449b14CAF01da6C)
- `PriceOracle`
  - [`0x6385892aCB085eaa24b745a712C9e682d80FF681`](https://etherscan.io/address/0x6385892aCB085eaa24b745a712C9e682d80FF681)
- `UniversalAdapter`
  - [`0xb460F4A66153bD3D059cEE424796EB213508d313`](https://etherscan.io/address/0xb460F4A66153bD3D059cEE424796EB213508d313)
  - [`0xBE7b6Fa3405C5CcCCDFA6Ef00Ec874c46dF96f0b`](https://etherscan.io/address/0xBE7b6Fa3405C5CcCCDFA6Ef00Ec874c46dF96f0b)
  - [`0xceD75810d1f0e3a977651b162f6e2d6F7A6A7572`](https://etherscan.io/address/0xceD75810d1f0e3a977651b162f6e2d6F7A6A7572)
  - [`0xB4724a5b053d3182B8ACa07484d77f72D687328b`](https://etherscan.io/address/0xB4724a5b053d3182B8ACa07484d77f72D687328b)
  - [`0xd3eDAAF68a5345C038d433af685d8aa43d9517b3`](https://etherscan.io/address/0xd3eDAAF68a5345C038d433af685d8aa43d9517b3)
  - [`0x2A22ADEe8D99dd88FE3140B43Ba59329529e14d6`](https://etherscan.io/address/0x2A22ADEe8D99dd88FE3140B43Ba59329529e14d6)
- `WETHGateway`
  - [`0x4F952c4C5415B2609899AbDC2F8F352F600d14D6`](https://etherscan.io/address/0x4F952c4C5415B2609899AbDC2F8F352F600d14D6)

### Integrations
