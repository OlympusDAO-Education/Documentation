# 본드

## DAI 본드

모든 채권 컨트랙트는 그들이 관리하는 자산이나 LP 토큰을 제외하고는 거의 같습니다. 본드 컨트랙트는 모든 예치와 상환을 처리합니다. 통화 정책에 필요한 파라미터들이 이 곳에 설정되어 있습니다. 이러한 파라미터들은 이를테면 [BCV](https://docs.olympusdao.finance/references/glossary#bcv) 그리고 최대 개인 지급액\(max individual payout\)이 있습니다. 아래를 통해 현재 활성화 되어있는 DAI의 최신 버전 컨트랙트를 확인하세요.

* V1 [0xa64E...2A3c](https://etherscan.io/address/0xa64ED1b66Cb2838Ef2A198D8345c0ce6967A2A3c)
* V2 [0xd030...f045](https://etherscan.io/address/0xd03056323b7a63e2095ae97fa1ad92e4820ff045)
* V3 [0x5754...381](https://etherscan.io/address/0x575409F8d77c12B05feD8B455815f0e54797381c)

## OHM / DAI LP 본드

* V1 [0xd270...ff29](https://etherscan.io/address/0xd27001d1aaed5f002c722ad729de88a91239ff29)
* V2 [0x13e8...8536](https://etherscan.io/address/0x13e8484a86327f5882d1340ed0d7643a29548536)
* V3 [0x9966...1626](https://etherscan.io/address/0x996668c46fc0b764afda88d83eb58afc933a1626)
* V4 [0x956c...c151](https://etherscan.io/address/0x956c43998316b6a2F21f89a1539f73fB5B78c151)

## OHM / FRAX LP 본드

* V1 [0x539b...3776](https://etherscan.io/address/0x539b6c906244ac34e348bbe77885cdfa994a3776)
* V2 [0xc20c...02f7](https://etherscan.io/address/0xc20cfff07076858a7e642e396180ec390e5a02f7)

## FRAX 본드

* V1 [0x8510...2514](https://etherscan.io/address/0x8510c8c2B6891E04864fa196693D44E6B6ec2514)

## ETH 본드

ETH 자체가 ERC-20 토큰은 아니기 때문에, ETH 본드는 [wETH](https://weth.io/)을 사용합니다. 모든 것들이 다른 본드의 형태와 동일하지만 한 가지 예외가 있다면 ETH 본드는 wETH를 근거로 OHM을 발행하지 않는다는 점입니다. 아래를 통해 현재 활성화 되어있는 ETH의 최신 버전 컨트랙트를 확인하세요.

* V1 [0x7464...d90d](https://etherscan.io/address/0x7464a65aa3fc15a625e2adfb8b340277d804d90d)
* V2 [0xE629...6F1c](https://etherscan.io/address/0xE6295201CD1ff13CeD5f063a5421c39A1D236F1c)

## 상환\(Redeem\) 도우미

상환 도우미 컨트랙트는 모든 활성화된 본드 컨트랙트 주소들과 함께 구성되어 있습니다.`redeemAll` 기능을 호출하면, 모든 상환 가능한 본드 보상들이 예정된 수령자들에게 상환됩니다. 아래를 통해 현재 활성화 되어있는 상환 도우미의 최신 버전 컨트랙트를 확인하세요.

* V1 [0xE1e8...819E](https://etherscan.io/address/0xE1e83825613DE12E8F0502Da939523558f0B819E)

