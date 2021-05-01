# Equations

## Staking

$$
deposit = withdrawal
$$

Swaps between OHM and sOHM during staking and unstaking are always honored
1:1. The amount of OHM deposited into the staking contract will always result
in the same amount of sOHM. And the amount of sOHM withdrawn from the staking
contract will always result in the same amount of OHM.

$$
rebase = 1 - ( ohmDeposits / sOHMOutstanding )
$$

The treasury deposits $OHM into the distributor. The distributor deposits $OHM
into the staking contract, creating an imbalance between $OHM and $sOHM. $sOHM
is rebased to correct this imbalance between $OHM deposited and $sOHM
outstanding. The rebase brings $sOHM outstanding back up to parity so that 1
$sOHM equals 1 staked $OHM.

## Bonding

Bond prices are determined by the value of the SLP and the number of bonds outstanding. The more bonds there are waiting to vest, the higher the premium on new bonds. This creates a secondary price discovery mechanism that is somewhat independent from the actual market.

$$
Bond Price = RFV / Premium
$$

The risk-free value is derived from the assets in the liquidity pool. The protocol sees OHM and DAI as equal because the protocol measures OHM by its intrinsic value. This means we only need to care about the sum of the assets in the pool and not their value. Based on the constant product formula x \* y = k, the risk free value is the minimum for x + y. This happens to be when x = y. We can use the square root of x \* y to determine this point.

$$
RFV=2sqrt(constantProduct) *(LP/totalLP)
$$

The debt ratio is the total of all OHM promised to bonds divided by the total supply of OHM. This allows us to measure the debt of the system.

$$
debt Ratio = bondsOutstanding/ohmSupply
$$

The premium is derived from the debt ratio of the system and a scaling variable. This scaling variable allows us to control the rate at which bond prices increase.

The premium determines profit due to the protocol and in turn stakers. \*\*\*\*The LP taken by the premium is used to mint and distribute new OHM to stakers and the DAO.

$$
Premium = 1 + (debt Ratio * n)
$$

## Sales

$$
executingPrice=lastMarketPrice*(1-discount)
$$

If the last market price is greater than the TWAP, the sales contract executes orders at that last market price minus a DAO-controlled discount which provides an arbitrage to encourage liquidity.

## Treasury

$$
IV = reserves/supply
$$

The intrinsic value is determined by total reserve assets divided by total OHM supply.

$$
profitMint =(IV-1)*supply
$$

At the end of each epoch, the treasury mints OHM so that IV returns to our intended value of 1.

$$
epochMint=(TWAP-IV)*supply*ICV
$$

If TWAP is greater than IV, the treasury uses this equation to fund the sales contract with OHM. ICV is a DAO-controlled scaling variable that allows us to tune inflation.

$$
epochBurn=|TWAP-IV|*supply*DCV
$$

If TWAP is less than IV, the treasury uses this equation to fund the sales contract with DAI. DCV is a DAO-controlled scaling variable that allows us to tune deflation.
