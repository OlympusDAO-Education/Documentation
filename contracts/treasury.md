# Treasury

## OHM / DAI LP

* V1 [0x34d7...ef7c](https://etherscan.io/address/0x34d7d7Aaf50AD4944B70B320aCB24C95fa2def7c)

## Treasury

The treasury contract is a simple vault implementation holding all the funds collected by the protocol. If for instance a user purchases a DAI bond, the bonded DAI is fully taken in by the treasury in return of the market equivalent of OHM bonded for. New OHM will be minted based on the RFV of the treasury assets. Below are listed treasury contracts by version, where the latest version represents the currently active contract.

* V1 [0x886C...399D](https://etherscan.io/address/0x886CE997aa9ee4F8c2282E182aB72A705762399D)
* V2 [0x31F8...46E8](https://etherscan.io/address/0x31F8Cc382c9898b273eff4e0b7626a6987C846E8)

The treasury contract is guarded by a 2 of 4 multisig. That means any transaction for the treasury must be approved by at least 2 signers, of which we have 4 signers in total. The operation security for our treasury assets is thus protected from a single actor going rogue, because it takes a quorum of 2 to authorize any transaction like moving funds in and out. Note that treasury and policy are guarded by the same signers. The 4 signing addresses for our treasury are listed below.

1. [0x1664...4033](https://etherscan.io/address/0x1664852674e93268Ef7704B7c345b20a876d4033)
2. [0x4Da7...091C](https://etherscan.io/address/0x4Da7EB21fd6c918b57f61B15109133C069FA091C)
3. [0xe643...812D](https://etherscan.io/address/0xe6435E2D1De6e3D3a9e90B2e80e7956ce59A812D)
4. [0x8d34...290E](https://etherscan.io/address/0x8d34EA6fb1Ed6B60F94ac6CD01dD1181ef12290E)
5. [0x3524...7dd3](https://etherscan.io/address/0x3524c03D39A13D51485419A17586286A6b617dd3)

