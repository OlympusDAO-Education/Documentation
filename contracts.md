# Contracts

## OHM

https://etherscan.io/address/0x383518188c0c6d7730d91b2c03a03c837814a899

If you want to buy OHM on Sushiswap or any other DEX please make sure the token
address of the token you purchase matches the one shown above. Never buy any OHM
token which address you cannot verify yourself. Further, knowing the OHM token
address you can see the list of holders and available exchanges providing
liquidity for OHM on Etherscan.

## sOHM

https://etherscan.io/address/0x04f2694c8fcee23e8fd0dfea1d4f5bb8c352111f

You receive sOHM when you stake OHM at a 1:1 ratio. Adding this address to your
wallet allows you to track your sOHM balance which increases with every rebase.
Below are listed old sOHM contracts which got phased out due to historical
reasons.

- V1 [0x3193...Fbbe](https://etherscan.io/address/0x31932E6e45012476ba3A3A4953cbA62AeE77Fbbe)
- V2 [0x04f2...111f](https://etherscan.io/address/0x04f2694c8fcee23e8fd0dfea1d4f5bb8c352111f)

## aOHM

https://etherscan.io/address/0x24ecfd535675f36ba1ab9c5d39b50dc097b0792e

When OlympusDAO first launched, alphaOHM (aOHM) was used as a pre-allocation
token which allowed the early participants to lay claim to OHM. Moving forward
aOHM will serve as the in-game currency of [Alpha Omega](https://medium.com/@alpha_omega/alpha-omega-a-tale-of-two-cities-80a94966376b),
a community-led social game that runs on the blockchain. Other than that aOHM is
not relevant to OHM or the operation of OlympusDAO.

## Staking

- new https://etherscan.io/address/0xFd31c7d00Ca47653c6Ce64Af53c1571f9C36566a
- helper https://etherscan.io/address/0xC8C436271f9A6F10a5B80c8b8eD7D0E8f37a612d
- old https://etherscan.io/address/0x0822F3C03dcc24d200AFF33493Dc08d0e1f274A2

## LP

https://etherscan.io/address/0x34d7d7Aaf50AD4944B70B320aCB24C95fa2def7c

## LP Staking

https://etherscan.io/address/0xF11f0F078BfaF05a28Eac345Bb84fcb2a3722223

## DAI Bond

https://etherscan.io/address/0xd03056323b7a63e2095ae97fa1ad92e4820ff045

All bond contracts are more or less the same, with the one exception of the
assets or LP tokens they manage. The bond contracts handle all deposits and
redemptions. Here parameters for monetary policy are configured. Such parameters
are for instance the [BCV](https://docs.olympusdao.finance/references/glossary#bcv)
and the max individual payout. Below are listed old DAI bond contracts which got
phased out due to historical reasons.

- V1 https://etherscan.io/address/0xa64ED1b66Cb2838Ef2A198D8345c0ce6967A2A3c
- V2 https://etherscan.io/address/0xd03056323b7a63e2095ae97fa1ad92e4820ff045
- V3 https://etherscan.io/address/0x575409F8d77c12B05feD8B455815f0e54797381c

## OHM / DAI LP Bond

- V1 https://etherscan.io/address/0xd27001d1aaed5f002c722ad729de88a91239ff29
- V2 https://etherscan.io/address/0x13e8484a86327f5882d1340ed0d7643a29548536
- V3 https://etherscan.io/address/0x996668c46fc0b764afda88d83eb58afc933a1626
- V4 https://etherscan.io/address/0x956c43998316b6a2F21f89a1539f73fB5B78c151

## OHM / FRAX LP Bond

- V1 https://etherscan.io/address/0x539b6c906244ac34e348bbe77885cdfa994a3776
- V2 https://etherscan.io/address/0xc20cfff07076858a7e642e396180ec390e5a02f7

## FRAX Bond

- V1 https://etherscan.io/address/0x8510c8c2B6891E04864fa196693D44E6B6ec2514


## Circulating Supply

https://etherscan.io/address/0x0efff9199aa1ac3c3e34e957567c1be8bf295034

This smart contract here is an intermediary component used to provide the
current circulating supply of OHM tokens. The [DAI Bond](#dai-bond) contract for
instance calls for the circulating supply in order to calculate the max payout
to stakers in every epoch. The [Distributor](#distributor) contract for instance
calls for the circulating supply in order to calculate the DAI bond debt ratio.

## Distributor

https://etherscan.io/address/0x73cfe6b116d161a2f9c165f7fc5270fb7dd2bb1e

The distributor contract receives minted OHM from the treasury in order to
drip-feed rewards to stakers. This means all OHM in the distributor is backed by
DAI, because it is already being accounted for by the protocol. The reward rate
as of time of writing is set to 5700, which translates to 0.57% of circulating
supply, since the reward rate is defined in tens of thousands. Note that the
reward rate determines the rebase rate and that the rebase rate determines the
APY. Below are listed old distributor contracts which got phased out due to
historical reasons.

- [0xbe73...242f](https://etherscan.io/address/0xbe731507810C8747C3E01E62c676b1cA6F93242f)
- [0xce65...f4c4](https://etherscan.io/address/0xce6568338708400d03f430d29f2eb40a33a3f4c4)

## Treasury

https://etherscan.io/address/0x31F8Cc382c9898b273eff4e0b7626a6987C846E8

The treasury contract is a simple vault implementation holding all the funds
collected by the protocol. If for instance a user purchases a DAI bond, the
bonded DAI is fully taken in by the treasury in return of the market equivalent
of OHM bonded for. New OHM will be minted based on the RFV of the treasury
assets. Below are listed old treasury contracts which got phased out due to
historical reasons.

- [0x886C...399D](https://etherscan.io/address/0x886CE997aa9ee4F8c2282E182aB72A705762399D)
