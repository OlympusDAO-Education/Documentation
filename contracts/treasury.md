# Treasury

## Treasury

The treasury contract is a simple vault implementation holding all the funds
collected by the protocol. If for instance a user purchases a DAI bond, the
bonded DAI is fully taken in by the treasury in return of the market equivalent
of OHM bonded for. New OHM will be minted based on the RFV of the treasury
assets. Below are listed treasury contracts by version, where the latest version
represents the currently active contract.

* V1 [0x886C...399D](https://etherscan.io/address/0x886CE997aa9ee4F8c2282E182aB72A705762399D)
* V2 [0x31F8...46E8](https://etherscan.io/address/0x31F8Cc382c9898b273eff4e0b7626a6987C846E8)
* V3 [0x9A31...13Ef](https://etherscan.io/address/0x9A315BdF513367C0377FB36545857d12e85813Ef)

The treasury contract is guarded by a 4 of 7 multisig. That means any
transaction for the treasury must be approved by at least 4 signers, of which we
have 7 signers in total. The operation security for our treasury assets is thus
protected from a single actor going rogue, because it takes a quorum of 4 to
authorize any transaction like moving funds in and out. The 7 signing addresses
for our treasury are listed below.

Note that the DAO and the Treasury signers are the same, since the DAO is the
manager of the Treasury contract.

1. [0x1774...55eB](https://etherscan.io/address/0x1774B6106d7E969d467396a5e90089FeaD6E55eB)
2. [0x131b...bf80](https://etherscan.io/address/0x131bd1A2827ccEb2945B2e3B91Ee1Bf736cCbf80)
3. [0x3524...7dd3](https://etherscan.io/address/0x3524c03D39A13D51485419A17586286A6b617dd3)
4. [0x8d34...290E](https://etherscan.io/address/0x8d34EA6fb1Ed6B60F94ac6CD01dD1181ef12290E)
5. [0x4Da7...091C](https://etherscan.io/address/0x4Da7EB21fd6c918b57f61B15109133C069FA091C)
6. [0x4702...47dC](https://etherscan.io/address/0x4702D39c499236A43654c54783c3f24830E247dC)
7. [0x17e0...c96e](https://etherscan.io/address/0x17e06ce6914E3969f7BD37D8b2a563890cA1c96e)
8. [0xf976...936b](https://etherscan.io/address/0xf97664376416E9379f2354DB444BFE3f00B6936b)
