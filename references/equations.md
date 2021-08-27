# 방정식

## 스테이

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

Every OHM in circulation is backed by the Olympus treasury. The assets in the treasury can be divided into two categories: stablecoin and non-stablecoin.

$$
treasuryBalance_{stablecoin} = RFV_{reserveBond} + RFV_{lpBond}
$$

The stablecoin balance in the treasury grows when bonds are sold. [RFV](https://docs.olympusdao.finance/references/glossary#rfv) is calculated differently for different bond types.

$$
RFV_{reserveBond} = assetSupplied
$$

For reserve bonds such as DAI bond and FRAX bond, the RFV simply equals to the amount of the underlying asset supplied by the bonder.

$$
RFV_{lpBond} = 2sqrt(constantProduct) * (\%\ ownership\ of\ the\ pool)
$$

For LP bonds such as OHM-DAI bond and OHM-FRAX bond, the RFV is calculated differently because the protocol needs to mark down its value. Why? The LP token pair consists of OHM, and each OHM in circulation will be backed by these LP tokens - there is a cyclical dependency. To safely guarantee all circulating OHM are backed, the protocol marks down the value of these LP tokens, hence the name _risk-free_ value \(RFV\).

