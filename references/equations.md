# 방정식

## 스테이크

$$
deposit = withdrawal
$$

스테이킹과 언스테이킹의 경우 OHM과 sOHM간의 스왑은 항상 1:1 비율이 적용됩니다. 스테이킹 컨트랙트에 예치된 OHM의 양은 sOHM의 양과 항상 동일합니다. 마찬가지로 스테이킹 컨트랙트로부터 인출된 sOHM의 양도 OHM의 양과 항상 동일합니다.

$$
rebase = 1 - ( ohmDeposits / sOHMOutstanding )
$$

금고는 OHM을 배급자 컨트랙트에 보관합니다. 그 다음 배급자는 OHM을 스테이킹 컨트랙트에 예치하여 OHM과 sOHM의 불균형을 만들어냅니다. sOHM은 예치된 OHM과 미지급된 sOHM 사이의 불균형을 해소하기 위해서 리베이싱 됩니다. 이 리베이싱을 통해 미지급된 sOHM을 동등하게 만들어서 1 sOHM이 1 스테이킹된 OHM과 같아집니다.

## 본

$$
bond Price = 1 + Premium
$$

OHM은 1 DAI 만큼의 내재가치를 가지며, 대략 $1에 해당합니다. 올림푸스는 본딩으로부터 수익을 내기 위해 각 본드마다 프리미엄을 부과합니다.

$$
Premium = debt Ratio * BCV
$$

이 프리미엄은 시스템의 부채비율, 그리고 BCV\(링크\)라고 불리는 확장 변수로부터 파생됩니다. BCV는 본드 가격의 상승을 조절할 수 있도록 만들어 줍니다.

프리미엄은 프로토콜과 스테이커들에 의해 수익이 결정됩니다. 왜냐하면 OHM은 수익을 통해 발행되고 이후 모든 스테이커들에게 배분되기 때문입니다.

$$
debt Ratio = bondsOutstanding/ohmSupply
$$

The debt ratio is the total of all OHM promised to bonders divided by the total supply of OHM. This allows us to measure the debt of the system.

$$
bondPayout_{reserveBond} = marketValue_{asset}\ /\ bondPrice
$$

본드 지급은 본드로 판매된 OHM의 수량을 결정합니다. 준비 본드\(링크\)의 경우, 본더에 의해 공급된 자산의 시장 가치는 본드 지급 결정을 위해 사용됩니다. 예를 들어, 만약 한 유저가 1000 DAI를 공급하고 본드 가격이 250 DAI라면, 유저는 4 OHM 만큼의 권리를 갖게 됩니다.

$$
bondPayout_{lpBond} = marketValue_{lpToken}\ /\ bondPrice
$$

유동성 본드\(링크\)의 경우, 본더에 의해 공급된 LP 토큰의 시장 가치는 본드 지급 결정을 위해 사용됩니다. 예를 들어 한 유저가 본딩 시점에서 1000 DAI 만큼의 가치를 지니는 0.001 OHM-DAI LP 토큰을 공급하고, 본드 가격이 250 DAI라면, 유저는 4 OHM 만큼의 권리를 갖게 됩니다.

## OHM 공급

$$
OHM_{supplyGrowth} = OHM_{stakers} + OHM_{bonders} + OHM_{DAO}
$$

OHM 공급량에는 하드캡이 없습니다. 아래와 같은 경우 증가합니다:

* OHM은 스테이커를 위해 발행되고 배분됩니다.
* OHM은 본더를 위해 발행됩니다. 이는 누군가 본드를 구매할 때 언제든 발생합니다.
* OHM은 DAO를 위해 발행됩니다. 이는 누군가 본드를 구매할때 언제든 발생합니다. DAO는 본더와 동일한 양의 OHM을 받습니다.

$$
OHM_{stakers} = OHM_{totalSupply} * rewardRate
$$

매 에포크의 마지막 마다, 금고는 정해진 보상 비율\(링크\)에 따라 OHM을 발행합니다. 이 OHM은 프로토콜에 있는 모든 스테이커들에게 배분됩니다. [올림푸스 정책 대시보드](https://dune.xyz/shadow/Olympus-Policy)를 통해 최신의 보상 비율을 확인할 수 있습니다.

$$
OHM_{bonders} = bondPayout
$$

누군가 본드를 구입하면, 언제든 정해진 수량의 OHM이 발행됩니다. 이 OHM들은 본더들에게 한 번에 배분되지 않습니다. 이것들은 선형적으로 시간에 따라 베스팅 됩니다. 본드 지급은 본드 타입에 따라 다른 공식을 사용합니다. 본드 섹션\(링크\)을 통해 어떻게 계산되는지 확인하세요.

$$
OHM_{DAO} = OHM_{bonders}
$$

DAO는 본더와 동일한 양의 OHM을 수령합니다. 이는 DAO의 수익이기도 합니다.

## OHM 지지\(backing\)

$$
OHM_{backing} = treasuryBalance_{stablecoin} + treasuryBalance_{otherAssets}
$$

순환되는 모든 OHM은 올림푸스 금고에 의해 지지되고 있습니다. 금고의 자산들은 2개의 카테고리로 분류될 수 있습니다: 스테이블코인과 논-스테이블 코인

$$
treasuryBalance_{stablecoin} = RFV_{reserveBond} + RFV_{lpBond}
$$

금고에 있는 스테이블코인의 잔고는 본드가 팔릴때 늘어납니다. RFV\(링크\)는 본드 타입에 따라 다르게 계산됩니다.

$$
RFV_{reserveBond} = assetSupplied
$$

DAI 본드나 FRAX 본드와 같은 준비 본드의 경우, RFV는 단순히 본드에 의해 공급된 자산의 총량과 동일합니다.

$$
RFV_{lpBond} = 2sqrt(constantProduct) * (\%\ ownership\ of\ the\ pool)
$$

OHM-DAI 본드나 OHM-FRAX 본드와 같은 LP 본드의 경우, 프로토콜이 그 가격을 낮게 측정해야 하기 때문에 RFV는 다른 방식으로 계산됩니다. 왜냐구요? LP 토큰의 쌍은 OHM으로 구성되어 있으며 각 순환중인 OHM은 이 LP 토큰들로부터 지지되고 있기 때문입니다. 여기에는 순환하는 의존성이 있습니다. 모든 순환중인 OHM이 확실하고 안전하게 지지되기 위해서는, 프로토콜이 LP 토큰의 가치를 낮게 측정해야 합니다. RFV의 뜻이 '무위험가치'인 만큼이요.

