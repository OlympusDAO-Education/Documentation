# 금고

## OHM / DAI LP

* V1 [0x34d7...ef7c](https://etherscan.io/address/0x34d7d7Aaf50AD4944B70B320aCB24C95fa2def7c)

## 금고\(Treasury\)

금고 컨트랙트는 프로토콜이 수집한 모든 자산을 보유하고 있는 단순한 저장소 입니다. 예를 들어 만약 한 사용자가 DAI 본드를 구입하면, 채권화된 DAI는 채권화된 만큼의 시장 가격의 OHM만큼 금고에 완전히 귀속됩니다. 새 OHM은 금고 자산의 RFV를 기준으로 발행됩니다. 아래를 통해 현재 활성화 되어있는 금고의 최신 버전 컨트랙트를 확인하세요.

* V1 [0x886C...399D](https://etherscan.io/address/0x886CE997aa9ee4F8c2282E182aB72A705762399D)
* V2 [0x31F8...46E8](https://etherscan.io/address/0x31F8Cc382c9898b273eff4e0b7626a6987C846E8)

금고 컨트랙트는 2/4 멀티시그에 의해 보호됩니다. 이는 금고에서 트랜젝션을 일으킬 경우 현재 4명의 서명자 중 2명의 서명자로부터 승인을 받아야 한다는 뜻입니다. 따라서 악의를 가진 한 명이 있더라도 금고의 자산을 빼내거나 받으려는 경우 트랜젝션 서명에 4개의 승인이 필요하므로 금고의 운영 보안이 유지될 수 있습니다. 금고를 위한 4개의 서명 주소는 아래와 같습니다.

1. [0x1774...55eB](https://etherscan.io/address/0x1774B6106d7E969d467396a5e90089FeaD6E55eB)
2. [0x131b...bf80](https://etherscan.io/address/0x131bd1A2827ccEb2945B2e3B91Ee1Bf736cCbf80)
3. [0x3524...7dd3](https://etherscan.io/address/0x3524c03D39A13D51485419A17586286A6b617dd3)
4. [0x8d34...290E](https://etherscan.io/address/0x8d34EA6fb1Ed6B60F94ac6CD01dD1181ef12290E)

