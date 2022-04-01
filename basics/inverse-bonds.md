# Inverse Bonds ([OIP-76](https://forum.olympusdao.finance/d/1020-oip-76-create-inverse-bond-policy-lever))

## What are inverse bonds?

Inverse bonds have been introduced as a protocol lever in [OIP-76](https://snapshot.org/#/olympusdao.eth/proposal/0xa544837835f3c4e681efba18d33623d4eb2acedec352dfc3c926a45902cd3612) 
as a way to support the price of OHM when below the backing per OHM. As their name suggests, 
one can think of inverse bonds as doing the "inverse" of what a regular bond does: 
instead of taking a treasury asset in exchange for OHM, **it takes in OHM in exchange for an asset from the treasury**. 

Here is a TL;DR on inverse bonds: 
- They buy your OHM in exchange for a backing asset from the treasury.
- They buy your OHM at a premium (slightly above market price) and then burn it.
- They buy your OHM at a slight discount to the backing per OHM, increasing the backing per remaining OHM.
- They have no vesting, meaning that the asset exchange is instant.
- They are only available while the OHM market price is below the backing per OHM.
- They are launched by the policy team.
- Their price is determined by the market.

## Why are these bonds being introduced?

The purpose of inverse bonds is to absorb some sell pressure for OHM, supporting its price while 
increasing the backing per OHM.

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
- The policy team will add and remove bonds based on market conditions and treasury composition.

## How many of these bonds will be available?

- Bonds have a limited capacity and are sold out once their capacity is reached.
- While the policy team is ultimately responsible for implementing inverse bonds, the lower the price of OHM compared to backing, the more capacity should be expected. 

## When will these bonds become available?

- The [Snapshot governance vote](https://snapshot.org/#/olympusdao.eth/proposal/0xa544837835f3c4e681efba18d33623d4eb2acedec352dfc3c926a45902cd3612) has passed and inverse bonds can now be used as a protocol lever.
- The policy team is responsible for their implementation, notably the timing of inverse bonds and their capacities.

## Where can I buy these bonds?

- You will be able to buy them on the [Olympus website](https://app.olympusdao.finance) but only on the Ethereum network.
- They will be offered only while OHM trades below the backing per OHM.

## How do these bonds affect the backing per OHM?

- The protocol acquires and burns OHM at a discount compared to backing per OHM.
- The revenues from inverse bonds increase the backing of all remaining OHM tokens.

## Do these bonds guarantee a price floor?

- No. They simply increase the backing per OHM and absorb some sell pressure.
- It is effectively the treasury acting as a whale buying OHM, supporting the market. 
  As this whale can effectively buy all the circulating OHM, it reinforces market confidence. 

## Can these bonds drain the treasury?

- The policy team decides how much OHM can be bonded in total.
- The policy team allocates the amount of payout assets upfront to safeguard the treasury.
- In terms of implementation, inverse bonds do not have direct access to treasury assets.

## Will the DAO itself bond OHM?

- No, OHM in DAO funds will not be used for inverse bonds.

## Are these bonds the same as a buyback?

While they seem similar there are notable differences:

- They absorb sell pressure because they buy OHM slightly above the market price.
- They reduce sell pressure further because they increase the backing per OHM.
- Their availability is limited to certain market conditions.
- The amount of OHM tokens that the protocol will acquire and burn is limited.
- Sales are driven by market demand and not by the protocol or the DAO, removing moral hazard.

## What is the backing per OHM?

- The USD value of the assets in the treasury is called “backing” or “reserves”.
- OHM in liquidity pairs does not count towards the backing.
- Locked assets like vlCVX and veFXS do not count towards the backing (for this purpose).
- That backing divided by the amount of OHM in circulation is the “backing per OHM”.
- The current backing can be found on the [Olympus dashboard](https://app.olympusdao.finance/#/dashboard) under “Liquid backing per OHM”.

## Example

- `ETH` inverse bond
- `$120` backing per OHM
- `$100` market price of OHM
- `$100` bond price
- `$105` payout per bond (`5%` premium over the market price of OHM)

→ Treasury takes in `$100 in OHM` in exchange for `$105 in ETH`, supporting the market by removing some sell pressure.  
→ That `OHM` is burnt.  
→ The treasury effectively pockets a revenue of `$15`, increasing the backing of the remaining OHM tokens.
