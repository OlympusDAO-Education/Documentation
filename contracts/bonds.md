# Bonds

## DAI Bond

Tous les contrats obligataires sont plus ou moins les mêmes, à l'exception des actifs ou des jetons de LP qu'ils gèrent. Les contrats obligataires gèrent tous les dépôts et les rachats. Les paramètres de la politique monétaire sont configurés ici. Ces paramètres sont par exemple la [BCV](https://app.gitbook.com/@olympusdao-1/s/olympusdocs/~/drafts/-MiWjJjeTgvj-6Lg0VjZ/v/francais/basics/glossary/@drafts#bcv) et le paiement individuel maximum. Les contrats obligataires DAI sont listés ci-dessous par version, la dernière version représentant le contrat actuellement actif.

* V1 [0xa64E...2A3c](https://etherscan.io/address/0xa64ED1b66Cb2838Ef2A198D8345c0ce6967A2A3c)
* V2 [0xd030...f045](https://etherscan.io/address/0xd03056323b7a63e2095ae97fa1ad92e4820ff045)
* V3 [0x5754...381c](https://etherscan.io/address/0x575409F8d77c12B05feD8B455815f0e54797381c)

## OHM / DAI LP Bond

* V1 [0xd270...ff29](https://etherscan.io/address/0xd27001d1aaed5f002c722ad729de88a91239ff29)
* V2 [0x13e8...8536](https://etherscan.io/address/0x13e8484a86327f5882d1340ed0d7643a29548536)
* V3 [0x9966...1626](https://etherscan.io/address/0x996668c46fc0b764afda88d83eb58afc933a1626)
* V4 [0x956c...c151](https://etherscan.io/address/0x956c43998316b6a2F21f89a1539f73fB5B78c151)

## OHM / FRAX LP Bond

* V1 [0x539b...3776](https://etherscan.io/address/0x539b6c906244ac34e348bbe77885cdfa994a3776)
* V2 [0xc20c...02f7](https://etherscan.io/address/0xc20cfff07076858a7e642e396180ec390e5a02f7)

## FRAX Bond

* V1 [0x8510...2514](https://etherscan.io/address/0x8510c8c2B6891E04864fa196693D44E6B6ec2514)

## ETH Bond

Puisque ETH n'est pas un jeton ERC-20, nos obligations ETH utilisent wETH. Toutes choses étant égales à nos autres types d'obligations, la seule exception pour les obligations ETH est qu'il n'y pas de mint OHM contre le wETH pris au départ. Vous trouverez ci-dessous la liste des contrats d'obligations ETH par version, où la dernière version représente le contrat actuellement actif.

* V1 [0x7464...d90d](https://etherscan.io/address/0x7464a65aa3fc15a625e2adfb8b340277d804d90d)
* V2 [0xE629...6F1c](https://etherscan.io/address/0xE6295201CD1ff13CeD5f063a5421c39A1D236F1c)

## Redeem Helper

Le contrat d'aide au rachat est configuré avec toutes les adresses de contrats d'obligations actives. Lors de l'appel de`redeemAll,` toutes les récompenses en obligations pouvant être réclamées sont rachetées pour le bénéficiaire. Vous trouverez ci-dessous une liste des contrats d'aide au rachat par version, la dernière version représentant le contrat actuellement actif.

* V1 [0xE1e8...819E](https://etherscan.io/address/0xE1e83825613DE12E8F0502Da939523558f0B819E)

