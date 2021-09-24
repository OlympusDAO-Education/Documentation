# FAQ

## Why do I want to use Olympus Pro?

It allows you to buy your favorite DeFi tokens at a discounted rate. Besides, you are helping the protocol to [accumulate their own liquidity](../intro.md#benefits-of-olympus-pro-for-protocols) in the process. This keeps your goal and the protocol's aligned.

## What is the relationship between Olympus Pro and OlympusDAO?

Olympus Pro is a service offered by [OlympusDAO](https://www.olympusdao.finance/#/). OlympusDAO provides infrastructure, expertise, and exposure to other protocols in setting up the bond mechanism in exchange for a fee.

## Do I receive OHM from Olympus Pro bonds?

You do not receive OHM from Olympus Pro bonds. Instead, you get the native governance token the protocol offers. For example, protocol X would reward bonds in X instead of OHM.

## How is the bond price/discount determined? 

The bond discount is determined by the following formula:

$$
bondDiscount = (marketPrice - bondPrice)\ /\ marketPrice
$$

The bond price is determined by the debt ratio of the system and a scaling variable called the Bond Control Variable \([BCV](https://docs.olympusdao.finance/references/glossary#bcv)\). This allows us to control the rate at which the bond price increases. Note that the bond price is independent of the market price, as no data from price oracles are used when determining the bond price. 

$$
bondPrice = debtRatio * BCV
$$

The debt ratio is the amount of reward tokens owed to the bonders by the protocol, divided by the total supply of the reward tokens. A higher debt ratio implies a huge demand for bonds, resulting in a higher bond price, and vice versa.

$$
debtRatio = tokenOwed\ /\ tokenSupply
$$

## What is the catch? Buying tokens at a discount sounds too good to be true.

Tokens purchased through a bond are not released to the bonder all at once. Instead, they vest linearly over time. This prevents the bonder from selling their tokens all at once for a quick profit.

## What parameters can be adjusted?

### BCV

BCV directly affects the bond price - the higher the BCV, the higher the bond price. As a higher bond price makes bonds less attractive, the protocol can adjust this value to tune the bond capacity.

### Maximum Bond Size

This controls the maximum amount of reward tokens a user can purchase through a bond. It is set as a percentage of the total supply and typically ranges between 0.03-0.05% of the total supply.

### Bond Vesting Term

A bond vests linearly to the bonder over a length of time, called the bond vesting term. This means the bonder can claim a portion of the reward tokens each day, with all rewards being claimable at the end of the term.

