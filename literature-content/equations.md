# Equations

## Staking

$$
deposit = withdrawal
$$

Swaps between OHM and sOHM during staking and unstaking are always honored 1:1. The amount of OHM deposited into the staking contract will always result in the same amount of sOHM. And the amount of sOHM withdrawn from the staking contract will always result in the same amount of OHM.

$$
rebase = 1 - ( ohmDeposits / sOHMOutstanding )
$$

The treasury deposits OHM into the distributor. The distributor then deposits OHM into the staking contract, creating an imbalance between OHM and sOHM. sOHM is rebased to correct this imbalance between OHM deposited and sOHM outstanding. The rebase brings sOHM outstanding back up to parity so that 1 sOHM equals 1 staked OHM.

## Bonding

$$
bond Price = 1 + Premium
$$

OHM has an intrinsic value of 1 DAI, which is roughly equivalent to $1. In order to make a profit from bonding, Olympus charges a premium for each bond.

$$
Premium = debt Ratio * BCV
$$

The premium is derived from the debt ratio of the system and a scaling variable called [BCV](https://docs.olympusdao.finance/references/glossary#bcv). BCV allows us to control the rate at which bond prices increase.

The premium determines profit due to the protocol and in turn, stakers. This is because new OHM is minted from the profit and subsequently distributed among all stakers.

$$
debt Ratio = bondsOutstanding/ohmSupply
$$

The debt ratio is the total of all OHM promised to bonders divided by the total supply of OHM. This allows us to measure the debt of the system.

$$
bondPayout_{reserveBond} = marketValue_{asset}\ /\ bondPrice
$$

Bond payout determines the number of OHM sold to a bonder. For [reserve bonds](https://docs.olympusdao.finance/references/glossary#reserve-bonds), the market value of the assets supplied by the bonder is used to determine the bond payout. For example, if a user supplies 1000 DAI and the bond price is 250 DAI, the user will be entitled 4 OHM.

$$
bondPayout_{lpBond} = marketValue_{lpToken}\ /\ bondPrice
$$

For [liquidity bonds](https://docs.olympusdao.finance/references/glossary#liquidity-bonds), the market value of the LP tokens supplied by the bonder is used to determine the bond payout. For example, if a user supplies 0.001 OHM-DAI LP token which is valued at 1000 DAI at the time of bonding, and the bond price is 250 DAI, the user will be entitled 4 OHM.

## OHM Supply

$$
OHM_{supplyGrowth} = OHM_{stakers} + OHM_{bonders} + OHM_{DAO} + OHM_{pohmExercise}
$$

OHM supply does not have a hard cap. Its supply increases when:

* OHM is minted and distributed to the stakers.
* OHM is minted for the bonder. This happens whenever someone purchases a bond.
* OHM is minted for the DAO. This happens whenever someone purchases a bond. The DAO gets the same number of OHM as the bonder.
* OHM is minted for the team, investors, advisors, or the DAO. This happens whenever

  the aforementioned party exercises their pOHM.

$$
OHM_{stakers} = OHM_{totalSupply} * rewardRate
$$

At the end of each epoch, the treasury mints OHM at a set [reward rate](https://docs.olympusdao.finance/references/glossary#reward-rate). These OHM will be distributed to all the stakers in the protocol. You can track the latest reward rate on the [Olympus Policy dashboard](https://dune.xyz/shadow/Olympus-Policy).

$$
OHM_{bonders} = bondPayout
$$

Whenever someone purchases a bond, a set number of OHM is minted. These OHM will not be released to the bonder all at once - they are vested to the bonder linearly over time. The bond payout uses a different formula for different types of bonds. Check the [bonding section above](equations.md#bonding) to see how it is calculated.

$$
OHM_{DAO} = OHM_{bonders}
$$

The DAO receives the same amount of OHM as the bonder. This represents the DAO profit.

$$
OHM_{pohmExercise} = pOHM + DAI
$$

The individual would supply 1 pOHM along with 1 DAI to mint 1 OHM. The pOHM is subsequently burned. Read [this Medium article](https://olympusdao.medium.com/what-is-poh-16b2c38a6cd6) for more information on pOHM.

## Backing per OHM

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

