# Contracts

## OHM

https://etherscan.io/address/0x383518188c0c6d7730d91b2c03a03c837814a899

If you want to buy OHM on Sushiswap or any other DEX please make sure the token
address of the token you purchase matches the one shown above. Never buy any OHM
token which address you cannot verify yourself. Further, knowing the OHM token
address you can see the list of holders and available exchanges providing
liquidity for OHM on Etherscan.

## sOHM

https://etherscan.io/address/0x31932E6e45012476ba3A3A4953cbA62AeE77Fbbe

You receive sOHM when you stake OHM at a 1:1 ratio. Adding this address to your
wallet allows you to track your sOHM balance which increases with every rebase.

## aOHM

https://etherscan.io/address/0x24ecfd535675f36ba1ab9c5d39b50dc097b0792e

When OlympusDAO first launched, alphaOHM (aOHM) was used as a pre-allocation token which allowed the early participants to lay claim to OHM. Moving forward aOHM will serve as the in-game currency of [Alpha Omega](https://medium.com/@alpha_omega/alpha-omega-a-tale-of-two-cities-80a94966376b), a community-led social game that runs on the blockchain. Other than that aOHM is not relevant to OHM or the operation of OlympusDAO.

## Staking

https://etherscan.io/address/0x0822F3C03dcc24d200AFF33493Dc08d0e1f274A2

## LP

https://etherscan.io/address/0x34d7d7Aaf50AD4944B70B320aCB24C95fa2def7c

## LP Staking

https://etherscan.io/address/0xF11f0F078BfaF05a28Eac345Bb84fcb2a3722223

## DAI Bond

https://etherscan.io/address/0xa64ED1b66Cb2838Ef2A198D8345c0ce6967A2A3c

## LP Bond

https://etherscan.io/address/0x13E8484a86327f5882d1340ed0D7643a29548536

## Circulating Supply

https://etherscan.io/address/0x0efff9199aa1ac3c3e34e957567c1be8bf295034

## Distributor

https://etherscan.io/address/0xce6568338708400d03f430d29f2eb40a33a3f4c4

The distributor contract receives minted OHM from the treasury in order to
drip-feed rewards to stakers. This means all OHM in the distributor is backed by
DAI, because it is already being accounted for by the protocol. The reward rate
as of time of writing is set to 5700, which translates to 0.57% of circulating
supply, since the reward rate is defined in tens of thousands. Note that the
reward rate determines the rebase rate and that the rebase rate determines the
APY. Further note that the old distributor contract was at
[0xbe73...242f](https://etherscan.io/address/0xbe731507810C8747C3E01E62c676b1cA6F93242f)
due to historical reasons.

## Treasury

https://etherscan.io/address/0x886CE997aa9ee4F8c2282E182aB72A705762399D

The treasury contract is a simple vault implementation holding all the funds collected by
the protocol. If for instance a user purchases a DAI bond, the bonded DAI is
fully taken in by the treasury in return of the market equivalent of OHM bonded
for. Additional OHM minted is being sent to the distributor contract.
