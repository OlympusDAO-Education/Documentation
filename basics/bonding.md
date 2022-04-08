# Bonding

## What is bonding?

**Bonding is the secondary value accrual strategy of Olympus.** It allows Olympus
to acquire its own liquidity and reserve assets such as LUSD by selling OHM
at a discount in exchange for these assets. The protocol quotes the bonder with
terms such as the bond price, the amount of OHM tokens entitled to the bonder, and
the vesting term. 

In V1, the ohm payout was unstaked and vested linearly over the duration of the vesting period. 
**Starting with V2, the ohm payout is staked and claimable in full at the end of the bond.**
Note that V1 has been fully deprecated, and all the bonds running on our website are V2 bonds. 

**Bonding is an active, short-term strategy.** 
The price discovery mechanism of the bond market renders bond discounts more or less unpredictable. 
However, starting with V2, any bond that offers a positive discount (>=0%) outperforms pure staking (be sure to account for gas costs). 
Bonding is considered a more active investment strategy that has to be monitored but can be more profitable 
than staking.

**Bonding allows Olympus to accumulate its own liquidity.** 
We call our own liquidity [POL](../references/glossary.md#pol). 
More POL ensures there is always locked exit liquidity in our trading pools to facilitate market operations
and protect token holders. Olympus owning its own liquidity offers additional revenues for its treasury, on top
of additional confidence for OHM investors.

The decision of which assets to bond is for now taken by the policy team on behalf of the global DAO. The policy team's 
objective with bonds is to keep the purchasing power of OHM stable while maintaining sufficient liquidity. 
Pure on-chain governance for bonds is currenly actively explored within the DAO. 