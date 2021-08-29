# Borrowing

You can start by referring to David’s [Medium article on how to use Abracadabra](https://davidgmi.medium.com/how-to-cast-a-magic-spell-to-your-ohm-and-3-3-strategy-using-abracadabra-money-45fc6187f281) in addition to the basic explanations below.

{% hint style="warning" %}
Make sure you understand the risk of leveraging before proceeding.
{% endhint %}

## How to Borrow MIM

In [Pool 10](https://abracadabra.money/pool/10), You can borrow MIM using sOHM which is already staked in Olympus App. Details are below:

1. Connect your wallet and go to [Abracadabra.money Pool 10](https://abracadabra.money/pool/10).

2. Under the "WRAP" menu, wrap the amount of sOHM against which you want to borrow to wsOHM.

![](../../.gitbook/assets/screen-shot-2021-08-29-at-4.10.42-pm%20%281%29.png)

3. Move to "BORROW" menu, type the amount of wsOHM as you want to use as collateral, and type the amount of MIM you want to borrow.

{% hint style="info" %}
If this is your first interaction with the App, you need to approve the Abracadabra's contract to spend your token first. However, you only need to perform this once - subsequent wrapping or borrowing process doesn't require the token approval step.
{% endhint %}

**In case you don’t use leverage**

1. Liquidation price will be shown automatically based on your borrowing rate of $MIM, then ****be aware to borrow $MIM with signing in transaction.

**In case you use leverage**

![](../../.gitbook/assets/screen-shot-2021-08-29-at-4.10.54-pm%20%281%29.png)

1. Click on Change leverage’ and choose Looping rate
2. Looping rates differ between 1 to 10, it changes ‘amount of borrowing $MIM’, ‘leverage rate’, and ‘liquidation price’.
3. As Looping rate rises, the liquidation price also rises.
4. Better to use lower ‘Swap Tolerance’, but use proper % according to market circumstance. Suggesting to put lowest number to higher. It also occurs changes in liquidation price, and etc.
5. To use lower gas fee, click on ‘Update price’, and sign in transaction to borrow.

After you borrow, you can add more collateral before your collateral price approach to liquidation price. When your collaterals are liquidated, you’ll lose all of your assets so be careful.

