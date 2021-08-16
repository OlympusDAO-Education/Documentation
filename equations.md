# Equations

## Staking

$$
deposit = withdrawal
$$

Swaps between OHM and sOHM during staking and unstaking are always honored 1:1.
The amount of OHM deposited into the staking contract will always result in the
same amount of sOHM. And the amount of sOHM withdrawn from the staking contract
will always result in the same amount of OHM.

$$
rebase = 1 - ( ohmDeposits / sOHMOutstanding )
$$

The treasury deposits OHM into the distributor. The distributor then deposits
OHM into the staking contract, creating an imbalance between OHM and sOHM. sOHM
is rebased to correct this imbalance between OHM deposited and sOHM outstanding.
The rebase brings sOHM outstanding back up to parity so that 1 sOHM equals 1
staked OHM.

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

The debt ratio is the total of all OHM promised to bonders divided by the total
supply of OHM. This allows us to measure the debt of the system.

$$
bond Payout = RFV/bondPrice
$$

Bond payout determines the number of OHM sold to a bonder.

$$
RFV_{lpBond}=2sqrt(constantProduct) *(LP/totalLP)
$$

RFV, or risk-free value, depends on the bond type. For LP bond, it is derived from the assets in the liquidity pool. Take OHM-DAI pool for instance, the protocol sees OHM and DAI as equal because the protocol measures OHM by its intrinsic value. This means we only need to care about the sum of the assets in the pool and not their value. Based on the constant product formula x \* y = k, the risk free value is the minimum for x + y. This happens to be when x = y. We can use the square root of x \* y to determine this point.

$$
RFV_{bond} = assetSupplied
$$

For single-asset bonds such as DAI bond and FRAX bond, the RFV simply equals to the amount of the underlying asset supplied by the bonder.

## Treasury

$$
IV = \$1 of RFV + \% of farmed tokens + \% of wETH
$$

The IV (intrinsic value) of each OHM consists of $1 of [RFV](https://docs.olympusdao.finance/references/glossary#rfv), a percentage of farmed tokens (e.g. xSUSHI and stkAAVE), and a percentage of wETH sitting in the treasury.

The IV is dynamic - as the market values of the farmed tokens and wETH rise, so does the IV, but its floor is always guaranteed by the $1 of RFV. Also, as more assets are introduced to the treasury, the IV will be made up of these assets as well.

$$
profitMint =(IV-1)*supply
$$

At the end of each epoch, the treasury mints OHM so that IV returns to our
intended value of 1.

$$
epochBurn=|TWAP-IV|*supply*DCV
$$

If TWAP is less than IV, the treasury uses this equation to buy back OHM with DAI. DCV is a DAO-controlled scaling variable that allows us to
tune deflation.
