# 토큰

## 토큰&#x20;

### gOHM

gOHM은 거버넌스 OHM을 의미합니다. [v2 마이그레이션](../basics/v2.md)의 일환으로 gOHM이 [wsOHM](tokens.md#undefined)을 대체하게 됩니다. gOHM은 sOHM V2를 다른 블록체인에서 사용할 수 있게 해주는 랩트(Wrapped) sOHM V2 입니다. 가격은 wsOHM과 똑같은 방식으로 계산됩니다.&#x20;

sOHM을 보유했을 때와 마찬가지로 리베이스 수익을 받지만 가치의 증가는 사고 파는 시점의 현재 인덱스(Current Index) 값에 기반해서 이뤄지기 때문에 토큰의 수는 늘어나지 않습니다. 더 자세한 내용은 [FAQ](../basics/basics.md#how-do-i-track-my-rebase-rewards)를 참고하세요.

아래를 통해 현재 활성화 되어있는 최신 버전의 컨트랙트를 버전별로 확인하세요.

이더리움:

* V1 [0x0ab8...a52f](https://etherscan.io/address/0x0ab87046fBb341D058F17CBC4c1133F25a20a52f)

아비트럼 원:

* V1 [0x8D9b...5FB1](https://arbiscan.io/token/0x8D9bA570D6cb60C7e3e0F31343Efe75AB8E65FB1)

아발란체:

* V1 [0x321e...4251](https://snowtrace.io/token/0x321e7092a180bb43555132ec53aaa65a5bf84251)

팬텀:

* V1 [0x91fa...3FDc](https://ftmscan.com/token/0x91fa20244Fb509e8289CA630E5db3E9166233FDc)

폴리곤:

* V1 [0xd8cA...5195](https://polygonscan.com/token/0xd8cA34fd379d9ca3C6Ee3b3905678320F5b45195)

{% hint style="info" %}
**현재 인덱스에 대한 설명 / 마이그레이션 기간 동안 OHM이 적게 표시되는 이유는 무엇인가요?**

현재 인덱스는 프로토콜 출범 때 1 OHM을 스테이킹하고 지금까지 보유했다면 몇 OHM으로 불어났을지를 나타내는 값입니다. 현재 인덱스는 [올림푸스 대시보드](https://app.olympusdao.finance/#/dashboard)에서 확인할 수 있습니다.

V2로 마이그레이션하면 몇 개의 gOHM을 갖게될지 잘 모르겠다면 [FAQ](../basics/v2.md#gohm)를 읽어보세요.
{% endhint %}

### OHM

스시스왑이나 다른 DEX에서 OHM을 구입할 경우, 구입한 토큰의 토큰 주소가 아래의 것과 일치하는지 확인하세요. 확인이 안된 OHM은 절대 구입하지 마세요. 또한, OHM 토큰 주소를 알고 있으면 이더스캔에서 홀더 리스트와 OHM 유동성을 공급하는 거래소들을 볼 수 있습니다. 아래를 통해 현재 활성화 되어있는 최신 버전의 컨트랙트를 버전별로 확인하세요.

* V1 [0x3835...a899](https://etherscan.io/address/0x383518188c0c6d7730d91b2c03a03c837814a899)

### sOHM

여러분이 OHM을 스테이킹 할 경우 1:1 비율로 sOHM을 받습니다. 아래 주소를 지갑에 등록하여, 매 리베이스마다 증가하는 sOHM 잔고를 추적하세요. 아래를 통해 현재 활성화 되어있는 최신 버전의 컨트랙트를 버전별로 확인하세요.

* V1 [0x3193...Fbbe](https://etherscan.io/address/0x31932E6e45012476ba3A3A4953cbA62AeE77Fbbe)
* V2 [0x04f2...111f](https://etherscan.io/address/0x04f2694c8fcee23e8fd0dfea1d4f5bb8c352111f)

### wsOHM

wsOHM은 랩트(wrapped) sOHM 입니다. 논 리베이싱 랩퍼(non-rebasing wrapper)가 sOHM을 서로 다른 체인으로 전송될 수 있는 논 리베이싱 컨테이너(non-rebasing container)에 담는데 사용됩니다. 현재 이 토큰은 이더리움, 아비트럼, 아발란체 네트워크에서 사용할 수 있습니다. 아래를 통해 현재 활성화 되어있는 최신 버전의 컨트랙트를 버전별로 확인하세요. 주소를 추가할 때 **네트워크를 한 번 더 확인하세요**.

이더리움 메인넷:

* V1 [0xca76...3e65](https://etherscan.io/address/0xca76543cf381ebbb277be79574059e32108e3e65)

아비트럼 L2:

* V1 [0x739c...BC4B](https://arbiscan.io/token/0x739ca6d71365a08f584c8fc4e1029045fa8abc4b)

아발란체:

* V1 [0x8CD3...2073](https://cchain.explorer.avax.network/token/0x8CD309e14575203535EF120b5b0Ab4DDeD0C2073)

## 역사적인 토큰

아래 토큰들은 제네시스 블록 때부터 OHM을 가지고 있는 분들에게만 관련이 있습니다. 여전히 많은 이들이 이 토큰들에 관심을 가지고 있습니다.

### aOHM

alphaOHM(aOHM)은 올림푸스가 첫 런칭했을 때 초기 참여자들이 OHM을 받을 수 있도록 사용된 토큰입니다. 이 뿐 아니라 블록체인 위에서 작동하는 [Alpha Omega](https://medium.com/@alpha\_omega/alpha-omega-a-tale-of-two-cities-80a94966376b) 라는, 커뮤니티 주도의 소셜 게임 위에서 사용될 것입니다. 그 외에는 aOHM이 OHM이나 올림푸스와 연괸되어 있는 부분은 없습니다. 아래를 통해 현재 활성화 되어있는 최신 버전의 컨트랙트를 버전별로 확인하세요.

V1 [0x24ec...792e](https://etherscan.io/address/0x24ecfd535675f36ba1ab9c5d39b50dc097b0792e)

### pOHM

pOHM, pOLY라고도 알려졌던 이 토큰은 올림푸스의 프리세일 토큰입니다. 올림푸스를 부트스트랩 하기 위해 비공개 투자자들로부터 자금을 모으기 위해 사용되었습니다. 이것과 관련해서는 [미디엄 아티클](https://olympusdao.medium.com/what-is-poh-16b2c38a6cd6)에서 더 많은 내용을 볼 수 있습니다. 아래를 통해 현재 활성화 되어있는 pOHM의 최신 버전 컨트랙트를 확인하세요.

* V1 [0x3699...c800](https://etherscan.io/token/0x36994486c6e97c170065899d8659a28d7371c800)
