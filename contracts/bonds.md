# Bonds

## DAI Bond

All bond contracts are more or less the same, with the one exception of the
assets or LP tokens they manage. The bond contracts handle all deposits and
redemptions. Here parameters for monetary policy are configured. Such parameters
are for instance the
[BCV](https://docs.olympusdao.finance/references/glossary#bcv) and the max
individual payout. Below are listed DAI bond contracts by version, where the
latest version represents the currently active contract.

* V1 [0xa64E...2A3c](https://etherscan.io/address/0xa64ED1b66Cb2838Ef2A198D8345c0ce6967A2A3c)
* V2 [0xd030...f045](https://etherscan.io/address/0xd03056323b7a63e2095ae97fa1ad92e4820ff045)
* V3 [0x5754...381c](https://etherscan.io/address/0x575409F8d77c12B05feD8B455815f0e54797381c)

## ETH Bond

Since ETH is not an ERC-20 token itself, our ETH bonds utilize
[wETH](https://weth.io/). All things being equal to our other bond types, the
only exception for ETH bonds is that we do not mint OHM against wETH taken in to
begin with. Below are listed ETH bond contracts by version, where the latest
version represents the currently active contract.

* V1 [0x7464...d90d](https://etherscan.io/address/0x7464a65aa3fc15a625e2adfb8b340277d804d90d)
* V2 [0xE629...6F1c](https://etherscan.io/address/0xE6295201CD1ff13CeD5f063a5421c39A1D236F1c)

## FRAX Bond

* V1 [0x8510...2514](https://etherscan.io/address/0x8510c8c2B6891E04864fa196693D44E6B6ec2514)

## LUSD Bond

All bond contracts are more or less the same, with the one exception of the
assets or LP tokens they manage. The bond contracts handle all deposits and
redemptions. Here parameters for monetary policy are configured. Such parameters
are for instance the
[BCV](https://docs.olympusdao.finance/references/glossary#bcv) and the max
individual payout. Below are listed LUSD bond contracts by version, where the
latest version represents the currently active contract.

* V1 [0x10C0...D08D](https://etherscan.io/address/0x10C0f93f64e3C8D0a1b0f4B87d6155fd9e89D08D)

## OHM / DAI LP Bond

* V1 [0xd270...ff29](https://etherscan.io/address/0xd27001d1aaed5f002c722ad729de88a91239ff29)
* V2 [0x13e8...8536](https://etherscan.io/address/0x13e8484a86327f5882d1340ed0d7643a29548536)
* V3 [0x9966...1626](https://etherscan.io/address/0x996668c46fc0b764afda88d83eb58afc933a1626)
* V4 [0x956c...c151](https://etherscan.io/address/0x956c43998316b6a2F21f89a1539f73fB5B78c151)

## OHM / FRAX LP Bond

* V1 [0x539b...3776](https://etherscan.io/address/0x539b6c906244ac34e348bbe77885cdfa994a3776)
* V2 [0xc20c...02f7](https://etherscan.io/address/0xc20cfff07076858a7e642e396180ec390e5a02f7)

## OHM / LUSD LP Bond

All bond contracts are more or less the same, with the one exception of the
assets or LP tokens they manage. The bond contracts handle all deposits and
redemptions. Here parameters for monetary policy are configured. Such parameters
are for instance the
[BCV](https://docs.olympusdao.finance/references/glossary#bcv) and the max
individual payout. Below are listed OHM / LUSD LP bond contracts by version,
where the latest version represents the currently active contract.

* V1 [0xFB17...67b6](https://etherscan.io/address/0xFB1776299E7804DD8016303Df9c07a65c80F67b6)

## Redeem Helper

The redeem helper contract is configured with all active bond contract
addresses. When calling `redeemAll` all claimable bond rewards are redeemed for
the given recipient. Below are listed redeem helper contracts by version, where
the latest version represents the currently active contract.

* V1 [0xE1e8...819E](https://etherscan.io/address/0xE1e83825613DE12E8F0502Da939523558f0B819E)
