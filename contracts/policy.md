# Policy

## Policy

The policy contract is an address guarded by a simple gnosis safe implementation. The policy address manages adjustments of the monetary policy of the Olympus DAO protocol. This includes BCV and reward rate adjustments. Below are listed policy addresses by version, where the latest version represents the currently active address.

* V1 [0x0cf3...6b2E](https://etherscan.io/address/0x0cf30dc0d48604A301dF8010cdc028C055336b2E)

The policy contract is guarded by a 3 of 5 multisig. That means any transaction for making policy changes must be approved by at least 3 signers, of which we have 5 signers in total. The operation security for our monetary policy is thus protected from a single actor going rogue, because it takes a quorum of 3 to authorize any transaction like adjusting the reward rate. The 5 signing addresses for our monetary policy are listed below.

1. [0x1664...4033](https://etherscan.io/address/0x1664852674e93268Ef7704B7c345b20a876d4033)
2. [0x4Da7...091C](https://etherscan.io/address/0x4Da7EB21fd6c918b57f61B15109133C069FA091C)
3. [0xe643...812D](https://etherscan.io/address/0xe6435E2D1De6e3D3a9e90B2e80e7956ce59A812D)
4. [0x8d34...290E](https://etherscan.io/address/0x8d34EA6fb1Ed6B60F94ac6CD01dD1181ef12290E)
5. [0x3524...7dd3](https://etherscan.io/address/0x3524c03D39A13D51485419A17586286A6b617dd3)

