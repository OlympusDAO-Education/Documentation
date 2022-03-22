# Bonds

The rollout of [V2 bonds](https://olympusdao.medium.com/introducing-v2-bonds-a17c7da298a2)
requires a re-design of the bond contract. With this, V1 bonds have been
deprecated, but their contracts are still listed here for reference.

# V2 Bonds

There is only one V2 bond contract, which manages bonds of various types (e.g.
OHM-DAI LP bonds, FRAX bonds).

* [0x9025...1ef6](https://etherscan.io/address/0x9025046c6fb25fb39e720d97a8fd881ed69a1ef6)

# V1 Bonds

There are multiple V1 bond contracts, where each contract manages a single bond
type. Still, all bond contracts are more or less the same.

The bond contracts handle all deposits and
redemptions. Here parameters for monetary policy are configured. Such parameters
are for instance the
[BCV](https://docs.olympusdao.finance/references/glossary#bcv) and the max
individual payout.

The bond contracts are listed by version, where the latest version represents
the last active V1 bond contract. These are kept for reference.
Starting with V2, all bonds now share one address 
[0x9025...1ef6](https://etherscan.io/address/0x9025046c6fb25fb39e720d97a8fd881ed69a1ef6).

## DAI Bond

* V1 [0xa64E...2A3c](https://etherscan.io/address/0xa64ED1b66Cb2838Ef2A198D8345c0ce6967A2A3c)
* V2 [0xd030...f045](https://etherscan.io/address/0xd03056323b7a63e2095ae97fa1ad92e4820ff045)
* V3 [0x5754...381c](https://etherscan.io/address/0x575409F8d77c12B05feD8B455815f0e54797381c)

## CVX Bond

* V1 [0x6754...1920](https://etherscan.io/address/0x6754c69fe02178f54ADa19Ebf1C5569826021920)
* V2 [0x767e...e0a9](https://etherscan.io/address/0x767e3459a35419122e5f6274fb1223d75881e0a9)

## ETH Bond

Since ETH is not an ERC-20 token itself, our ETH bonds utilize
[wETH](https://weth.io/). 

* V1 [0x7464...d90d](https://etherscan.io/address/0x7464a65aa3fc15a625e2adfb8b340277d804d90d)
* V2 [0xE629...6F1c](https://etherscan.io/address/0xE6295201CD1ff13CeD5f063a5421c39A1D236F1c)

## FRAX Bond

* V1 [0x8510...2514](https://etherscan.io/address/0x8510c8c2B6891E04864fa196693D44E6B6ec2514)
* V2 [0xc60a...cc38](https://etherscan.io/address/0xc60a6656e08b62dd2644dc703d7855301363cc38)

## LUSD Bond

* V1 [0x10C0...D08D](https://etherscan.io/address/0x10C0f93f64e3C8D0a1b0f4B87d6155fd9e89D08D)

## OHM / DAI LP Bond

* V1 [0xd270...ff29](https://etherscan.io/address/0xd27001d1aaed5f002c722ad729de88a91239ff29)
* V2 [0x13e8...8536](https://etherscan.io/address/0x13e8484a86327f5882d1340ed0d7643a29548536)
* V3 [0x9966...1626](https://etherscan.io/address/0x996668c46fc0b764afda88d83eb58afc933a1626)
* V4 [0x956c...c151](https://etherscan.io/address/0x956c43998316b6a2F21f89a1539f73fB5B78c151)

## OHM / FRAX LP Bond

* V1 [0x539b...3776](https://etherscan.io/address/0x539b6c906244ac34e348bbe77885cdfa994a3776)
* V2 [0xc20c...02f7](https://etherscan.io/address/0xc20cfff07076858a7e642e396180ec390e5a02f7)
* V3 [0x99e9...aa53](https://etherscan.io/address/0x99e9b0a9dc965361c2cbc07525ea591761aeaa53)

## OHM / LUSD LP Bond

* V1 [0xFB17...67b6](https://etherscan.io/address/0xFB1776299E7804DD8016303Df9c07a65c80F67b6)

## Redeem Helper

The redeem helper contract is configured with all active bond contract
addresses. When calling `redeemAll` all claimable bond rewards are redeemed for
the given recipient. Below are listed redeem helper contracts by version for the V1 bonds. 
Starting with V2, all bonds can be redeemed calling `redeemAll` on the V2 bond contract
[0x9025...1ef6](https://etherscan.io/address/0x9025046c6fb25fb39e720d97a8fd881ed69a1ef6).

* V1 [0xE1e8...819E](https://etherscan.io/address/0xE1e83825613DE12E8F0502Da939523558f0B819E)
