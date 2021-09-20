# Staking

## Distributor

Le _distributor contract_ reçoit des OHM minted de la trésorie afin de distribuer des récompenses au compte-gouttes aux stakers. Au moment de la rédaction de ce document, le taux de récompense cible est fixé à 3500, ce qui correspond à 0,35% de l'offre totale, puisque le taux de récompense est défini en dizaines de milliers. Notez que le taux de récompense détermine le taux de rebasement et que le taux de rebasement détermine l'APY. Les contrats de distributeurs sont listés ci-dessous par version, la dernière version représentant le contrat actuellement actif.

* V1 [0xbe73...242f](https://etherscan.io/address/0xbe731507810C8747C3E01E62c676b1cA6F93242f)
* V2 [0xce65...f4c4](https://etherscan.io/address/0xce6568338708400d03f430d29f2eb40a33a3f4c4)
* V3 [0x73cf...bb1e](https://etherscan.io/address/0x73cfe6b116d161a2f9c165f7fc5270fb7dd2bb1e)
* V4 [0xc58e...3ce6](https://etherscan.io/address/0xc58e923bf8a00e4361fe3f4275226a543d7d3ce6)

## LP Staking

Le staking des LP est déprécié. Vous pouvez toujours débloquer votre LP via Etherscan.

* V1 [0xF11f...2223](https://etherscan.io/address/0xF11f0F078BfaF05a28Eac345Bb84fcb2a3722223)

## Staking

Avant la migration, l'ancien contrat de staking \([0x0822...74A2](https://etherscan.io/address/0x0822F3C03dcc24d200AFF33493Dc08d0e1f274A2)\) était utilisé pour le staking OHM. Si des utilisateurs sont encore sous contrat de staking, ils doivent migrer leurs OHM vers le nouveau contrat \([0xFd31....566a](https://etherscan.io/address/0xFd31c7d00Ca47653c6Ce64Af53c1571f9C36566a)\). Le nouveau contrat fonctionne avec un contrat d'aide au staking \([0xC8C4....612d](https://etherscan.io/address/0xC8C436271f9A6F10a5B80c8b8eD7D0E8f37a612d)\). Le contrat d'assistance au staking appelle "stake" et ensuite "claim" du nouveau contrat de staking. Lorsque la fonction "stake" est appelée, le sOHM est mis dans une phase de réchauffement et toutes les informations sur la quantité de sOHM qu'un utilisateur a stake sont stockées dans le nouveau contrat de staking. Lorsque la fonction "claim" est appelée, les sOHM sont récupérés et envoyés au portefeuille de l'utilisateur.

