# Contracts

## OHM

If you want to buy OHM on Sushiswap or any other DEX please make sure the token
address of the token you purchase matches the one shown above. Never buy any OHM
token which address you cannot verify yourself. Further, knowing the OHM token
address you can see the list of holders and available exchanges providing
liquidity for OHM on Etherscan. Below are listed OHM contracts by version, where
the latest version represents the currently active contract.

- V1 [0x3835...a899](https://etherscan.io/address/0x383518188c0c6d7730d91b2c03a03c837814a899)

## sOHM

You receive sOHM when you stake OHM at a 1:1 ratio. Adding this address to your
wallet allows you to track your sOHM balance which increases with every rebase.
Below are listed sOHM contracts by version, where the latest version represents
the currently active contract.

- V1 [0x3193...Fbbe](https://etherscan.io/address/0x31932E6e45012476ba3A3A4953cbA62AeE77Fbbe)
- V2 [0x04f2...111f](https://etherscan.io/address/0x04f2694c8fcee23e8fd0dfea1d4f5bb8c352111f)

## aOHM

When OlympusDAO first launched, alphaOHM (aOHM) was used as a pre-allocation
token which allowed the early participants to lay claim to OHM. Moving forward
aOHM will serve as the in-game currency of [Alpha Omega](https://medium.com/@alpha_omega/alpha-omega-a-tale-of-two-cities-80a94966376b),
a community-led social game that runs on the blockchain. Other than that aOHM is
not relevant to OHM or the operation of OlympusDAO. Below are listed aOHM
contracts by version, where the latest version represents the currently active
contract.

- V1 [0x24ec...792e](https://etherscan.io/address/0x24ecfd535675f36ba1ab9c5d39b50dc097b0792e)

## pOHM

pOHM, previously known as pOLY, is the presale token of Olympus. It was used to raise funds from private investors to bootstrap Olympus. You can read more about pOHM in this [Medium article](https://olympusdao.medium.com/what-is-poh-16b2c38a6cd6). Below are listed pOHM contracts by version, where the latest version represents the currently active contract.

- V1 [0x3699...c800](https://etherscan.io/token/0x36994486c6e97c170065899d8659a28d7371c800)

## Staking

Prior to the migration of the staking contract, the old staking contract
([0x0822...74A2](https://etherscan.io/address/0x0822F3C03dcc24d200AFF33493Dc08d0e1f274A2))
was used for staking OHM. If users are still staked in there they should migrate
their staked OHM to the new staking contract
([0xFd31....566a](https://etherscan.io/address/0xFd31c7d00Ca47653c6Ce64Af53c1571f9C36566a)).
The new staking contract works with a staking helper contract
([0xC8C4....612d](https://etherscan.io/address/0xC8C436271f9A6F10a5B80c8b8eD7D0E8f37a612d)).
The staking helper contract calls "stake" and then "claim" of the new staking
contract. When the "stake" function is called, sOHM is put into a warmup phase
and all the information about how much sOHM a user has staked is stored in the
new staking contract. When the "claim" function is called, sOHM is retrieved
from the warmup and then sent to the user's wallet.

## LP

- V1 [0x34d7...ef7c](https://etherscan.io/address/0x34d7d7Aaf50AD4944B70B320aCB24C95fa2def7c)

## LP Staking

- V1 [0xF11f...2223](https://etherscan.io/address/0xF11f0F078BfaF05a28Eac345Bb84fcb2a3722223)

## DAI Bond

All bond contracts are more or less the same, with the one exception of the
assets or LP tokens they manage. The bond contracts handle all deposits and
redemptions. Here parameters for monetary policy are configured. Such parameters
are for instance the [BCV](https://docs.olympusdao.finance/references/glossary#bcv)
and the max individual payout. Below are listed DAI bond contracts by version,
where the latest version represents the currently active contract.

- V1 [0xa64E...2A3c](https://etherscan.io/address/0xa64ED1b66Cb2838Ef2A198D8345c0ce6967A2A3c)
- V2 [0xd030...f045](https://etherscan.io/address/0xd03056323b7a63e2095ae97fa1ad92e4820ff045)
- V3 [0x5754...381c](https://etherscan.io/address/0x575409F8d77c12B05feD8B455815f0e54797381c)

## OHM / DAI LP Bond

- V1 [0xd270...ff29](https://etherscan.io/address/0xd27001d1aaed5f002c722ad729de88a91239ff29)
- V2 [0x13e8...8536](https://etherscan.io/address/0x13e8484a86327f5882d1340ed0d7643a29548536)
- V3 [0x9966...1626](https://etherscan.io/address/0x996668c46fc0b764afda88d83eb58afc933a1626)
- V4 [0x956c...c151](https://etherscan.io/address/0x956c43998316b6a2F21f89a1539f73fB5B78c151)

## OHM / FRAX LP Bond

- V1 [0x539b...3776](https://etherscan.io/address/0x539b6c906244ac34e348bbe77885cdfa994a3776)
- V2 [0xc20c...02f7](https://etherscan.io/address/0xc20cfff07076858a7e642e396180ec390e5a02f7)

## FRAX Bond

- V1 [0x8510...2514](https://etherscan.io/address/0x8510c8c2B6891E04864fa196693D44E6B6ec2514)

## ETH Bond

Since ETH is not an ERC-20 token itself, our ETH bonds utilize [wETH](https://weth.io/). All
things being equal to our other bond types, the only exception for ETH bonds is
that we do not mint OHM against wETH taken in to begin with. Below are listed
ETH bond contracts by version, where the latest version represents the currently
active contract.

- V1 [0x7464...d90d](https://etherscan.io/address/0x7464a65aa3fc15a625e2adfb8b340277d804d90d)
- V2 [0xE629...6F1c](https://etherscan.io/address/0xE6295201CD1ff13CeD5f063a5421c39A1D236F1c)

## Circulating Supply

This smart contract here is an intermediary component used to provide the
current circulating supply of OHM tokens. The [DAI Bond](#dai-bond) contract for
instance calls for the circulating supply in order to calculate the max payout
to stakers in every epoch. The [Distributor](#distributor) contract for instance
calls for the circulating supply in order to calculate the DAI bond debt ratio.
Below are listed circulating supply contracts by version, where the latest
version represents the currently active contract.

- V1 [0x0eff...5034](https://etherscan.io/address/0x0efff9199aa1ac3c3e34e957567c1be8bf295034)

## Distributor

The distributor contract receives minted OHM from the treasury in order to
drip-feed rewards to stakers. The reward rate target as of time of writing is
set to 3500, which translates to 0.35% of total supply, since the reward rate is
defined in tens of thousands. Note that the reward rate determines the rebase
rate and that the rebase rate determines the APY. Below are listed distributor
contracts by version, where the latest version represents the currently active
contract.

- V1 [0xbe73...242f](https://etherscan.io/address/0xbe731507810C8747C3E01E62c676b1cA6F93242f)
- V2 [0xce65...f4c4](https://etherscan.io/address/0xce6568338708400d03f430d29f2eb40a33a3f4c4)
- V3 [0x73cf...bb1e](https://etherscan.io/address/0x73cfe6b116d161a2f9c165f7fc5270fb7dd2bb1e)
- V4 [0xc58e...3ce6](https://etherscan.io/address/0xc58e923bf8a00e4361fe3f4275226a543d7d3ce6)

## Redeem Helper

The redeem helper contract is configured with all active bond contract
addresses. When calling `redeemAll` all claimable bond rewards are redeemed for
the given recipient. Below are listed redeem helper contracts by version, where
the latest version represents the currently active contract.

- V1 [0xE1e8...819E](https://etherscan.io/address/0xE1e83825613DE12E8F0502Da939523558f0B819E)

## Treasury

The treasury contract is a simple vault implementation holding all the funds
collected by the protocol. If for instance a user purchases a DAI bond, the
bonded DAI is fully taken in by the treasury in return of the market equivalent
of OHM bonded for. New OHM will be minted based on the RFV of the treasury
assets. Below are listed treasury contracts by version, where the latest version
represents the currently active contract.

- V1 [0x886C...399D](https://etherscan.io/address/0x886CE997aa9ee4F8c2282E182aB72A705762399D)
- V2 [0x31F8...46E8](https://etherscan.io/address/0x31F8Cc382c9898b273eff4e0b7626a6987C846E8)
