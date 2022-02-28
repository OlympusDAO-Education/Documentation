# Staking

## Distributor

The distributor contract receives minted OHM from the treasury in order to drip-feed rewards to stakers. The reward rate target as of time of writing is set to 3500, which translates to 0.35% of total supply, since the reward rate is defined in tens of thousands. Note that the reward rate determines the rebase rate and that the rebase rate determines the APY. Below are listed distributor contracts by version, where the latest version represents the currently active contract.

* V1 [0xbe73...242f](https://etherscan.io/address/0xbe731507810C8747C3E01E62c676b1cA6F93242f)
* V2 [0xce65...f4c4](https://etherscan.io/address/0xce6568338708400d03f430d29f2eb40a33a3f4c4)
* V3 [0x73cf...bb1e](https://etherscan.io/address/0x73cfe6b116d161a2f9c165f7fc5270fb7dd2bb1e)
* V4 [0xc58e...3ce6](https://etherscan.io/address/0xc58e923bf8a00e4361fe3f4275226a543d7d3ce6)

## LP Staking

LP staking is deprecated. You can unstake your LP via Etherscan still.

* V1 [0xF11f...2223](https://etherscan.io/address/0xF11f0F078BfaF05a28Eac345Bb84fcb2a3722223)

## Staking

Prior to [V1.1  migration](https://olympusdao.medium.com/olympus-v1-1-a5c6a48be7d1),
the old staking contract (V1) was used for staking OHM. Afterwards, a new staking
contract (V2) was rolled out, which  works with a staking helper (V2, Staking Helper).
The staking helper contract calls "stake" and then "claim" of the new staking contract.
When the "stake" function is called, sOHM is put into a warmup phase and all the
information about how much sOHM a user has staked is stored in the new staking
contract. When the "claim" function is called, sOHM is retrieved from the warmup
and then sent to the user's wallet.

As part of the [V2 migration](https://olympusdao.medium.com/get-ready-for-olympus-v2-migration-360764a61168),
a new staking contract (V3) has been rolled out, which supersedes the old staking
contract and the staking helper. It supports both staking and unstaking operations.

* V1 [0x0822...74A2](https://etherscan.io/address/0x0822F3C03dcc24d200AFF33493Dc08d0e1f274A2)
* V2 [0xFd31....566a](https://etherscan.io/address/0xFd31c7d00Ca47653c6Ce64Af53c1571f9C36566a)
* V2, Staking Helper [0xC8C4....612d](https://etherscan.io/address/0xC8C436271f9A6F10a5B80c8b8eD7D0E8f37a612d)
* V3 [0xB63c...8020](https://etherscan.io/address/0xB63cac384247597756545b500253ff8E607a8020)
