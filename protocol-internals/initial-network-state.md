# Initial Network State

**Our initial goal is not to find a stable price.** This may seem antithetical to our currency aspirations, but we ensure you it is not. Olympus can be tuned to optimize for different things. The main tradeoff is volatility and profitability versus stability and consistency. With volatility and profit comes growth; this is what we want early on.

With tight policy and scale, Olympus should function well as a stable asset. Upward and downward pressures should stabilize at some non-intrinsic value. With loose policy, regardless of scale, Olympus has the potential to act as a wealth creation machine. The market premium of the token measures the positive sum of the game; all extrinsic value is new wealth created.

## Alpha State

The initial network features a one-way treasury \(money goes in, none comes out\), the bonding contract \(through which supply increases and profits are produced\), and the staking contract \(where profits are distributed\).

The following are the initial policy states:

* **BCV**

  [BCV](https://docs.olympusdao.finance/references/glossary#bcv) varies based on bond types. It is tuned regularly by the Policy team to meet the protocol goals. For example, if the protocol wants to accumulate more liquidity into its treasury, it can lower the BCV for [liquidity bonds](https://docs.olympusdao.finance/references/glossary#liquidity-bonds) to increase their bond capacity. To view the BCV targets for different bond types, visit the [Olympus Policy Dune page](https://dune.xyz/shadow/Olympus-Policy).

* **Bond vesting term**

  It is set to 33110 Ethereum blocks or approximately five days for all bond types.

* **OHM distribution**

  Every time someone purchases a bond, the proceed will go to the [Olympus treasury](https://docs.olympusdao.finance/references/contracts#treasury). A corresponding amount of OHM will be minted and distributed to three parties:

  * Bonder

    The bond purchaser will receive the quoted amount of OHM linearly over the vesting term.

  * DAO

    The DAO receives the same amount of OHM as the bonder. This represents the DAO profit.

  * Stakers

    After accounting for the OHM distributed to the bonder and the DAO, the rest will be distributed among all stakers in the protocol.

