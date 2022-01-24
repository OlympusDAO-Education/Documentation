# Inverse Bonds ([OIP-76](https://forum.olympusdao.finance/d/1020-oip-76-create-inverse-bond-policy-lever))

## What are inverse bonds?

- They buy your OHM and sell you a backing asset from the treasury.
- They buy your OHM at a premium (slightly above market price) and then burn it.
- They have no vesting and the asset exchange is instant.
- They are only available while the OHM market price is below the backing per OHM.
- They are launched by the policy team.
- Their price is determined by the market.

## Why are these bonds being introduced?

- The policy team enacts monetary policy to support the health of the protocol.
- Inverse bonds are an additional tool for the policy team to do that effectively.
- They allow OHM to be sold without directly affecting its market price.
- Their purpose is
    - to absorb some sell pressure for OHM.
    - to increase the backing per OHM.
- They mirror the properties of regular bonds that have been incredibly effective.

## What assets can I bond?

- You can bond only OHM v2.
- You must unstake your sOHM or gOHM first.

## How much will these bonds cost?

- Their pricing mechanic is basically the same as for regular bonds:
    - The price and payout value of an inverse bond start at the market price of OHM.
    - The payout amount (premium) slowly increases until someone buys a bond.
    - The payout amount (premium) is then reduced and will slowly increase again.
- They will effectively buy OHM at a premium – slightly above market price.
- You will get more value for your OHM compared to selling directly to the market.

## What asset will I get for these bonds?

- Different bonds will be provided that pay out different assets.
- The policy team will add and remove bonds based on market conditions.

## How many of these bonds will be available?

- Bonds have a limited capacity and are sold out once their capacity is reached.
- Bond capacity will be determined by the policy team based on market conditions.

## When will these bonds become available?

- First they need to pass the [vote in the Olympus forum](https://forum.olympusdao.finance/d/1020-oip-76-create-inverse-bond-policy-lever).
- Next they need to pass the [Snapshot governance vote](https://snapshot.org/#/olympusdao.eth/proposal/0xa544837835f3c4e681efba18d33623d4eb2acedec352dfc3c926a45902cd3612).
- After the vote a modified version of v2 bonds will be deployed for inverse bonds.
- Finally, the policy team will decide if and when inverse bonds will be made available.

## Where can I buy these bonds?

- You will be able to buy them on the [Olympus website](https://app.olympusdao.finance) but only on the Ethereum network.
- They will be offered only while OHM trades below the backing per OHM.

## How do these bonds affect the backing per OHM?

- The protocol acquires and burns OHM for a fraction of the backing per OHM.
- The remaining fraction of the backing increases the backing of all other OHM tokens.

## How do these bonds effect the runway?

- Bonds that pay out risk-free assets will shorten the runway.
- Bonds that pay out other assets will extend the runway.

## Do these bonds guarantee a price floor?

- No. They simply increase the backing per OHM and absorb some sell pressure.
- That has a positive effect on the market price of OHM.

## Can these bonds drain the treasury?

- The policy team decides how much OHM can be bonded in total.
- The policy team allocates the amount of payout assets upfront to safeguard the treasury.
- Inverse bonds do not have direct access to treasury assets.

## Will the DAO itself bond OHM?

- No, OHM in DAO funds will not be used for inverse bonds.

## Why are they called "inverse" bonds?

- Regular [bonds](./bonding.md) take in treasury assets in exchange for OHM.
- Inverse bonds take in OHM in exchange for treasury assets, so the _inverse_.

## Are these bonds the same as a buyback?

While they seem similar there are notable differences:

- They absorb sell pressure because they buy OHM slightly above the market price.
- They reduce sell pressure further because they increase the backing per OHM.
- Their availability is limited to certain market conditions.
- The amount of OHM tokens that the protocol will acquire and burn is limited.
- Sales are driven by market demand and not by the protocol or the DAO.

## What is the backing per OHM?

- The USD value of the assets in the [treasury](https://zapper.fi/bundle/0x9a315bdf513367c0377fb36545857d12e85813ef,0xde7b85f52577B113181921A7aa8Fc0C22e309475,0xDbf0683fC4FC8Ac11e64a6817d3285ec4f2Fc42d,0x31f8cc382c9898b273eff4e0b7626a6987c846e8,0x408a9a09d97103022f53300a3a14ca6c3ff867e8,0x10B569271912CD3342d183c0f2dC4b5D5880b741,0x0e1177e47151be72e5992e0975000e73ab5fd9d4,0x0316508a1b5abf1cae42912dc2c8b9774b682ffc,0xe06efA3D9Ee6923240ee1195A16ddd96B5CcE8F7,0x2bC001fFEB862d843e0a02a7163C7d4828e5FB10,0xdfc95aaf0a107daae2b350458ded4b7906e7f728?label=Olympus%20Treasury) is called “backing” or “reserves”.
- OHM in liquidity does not count towards the backing.
- Locked assets like vlCVX and veFXS do not count towards the backing (for this purpose).
- That backing divided by the amount of OHM in circulation is the “backing per OHM”.
- The current backing can be found in the [Olympus Lookout](https://dune.xyz/fluidsonic/Olympus-DAO) dashboard under “Backing”.  
  Note that the backing on the dashboard is higher as it does include locked assets.

## Example

- `ETH` inverse bond
- `$120` backing per OHM
- `$100` market price of OHM
- `$100` bond price
- `$105` payout per bond (`5%` premium over the market price of OHM)

→ Treasury takes in `$100 in OHM` in exchange for `$105 in ETH`.  
→ That `OHM` is burnt.  
→ `$15` of backing can be allocated to the remaining OHM tokens, increasing overall backing.
