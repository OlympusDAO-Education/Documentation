# Borrowing

You can start by referring to David’s [Medium article on how to use Abracadabra](https://davidgmi.medium.com/how-to-cast-a-magic-spell-to-your-ohm-and-3-3-strategy-using-abracadabra-money-45fc6187f281) in addition to the basic explanations below.

{% hint style="warning" %}
Make sure you understand how leverage works in [this article from Abracadabra](https://docs.abracadabra.money/intro/leveraged-positions).
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

## **How to Leverage**

![](../../.gitbook/assets/screen-shot-2021-08-29-at-4.10.54-pm%20%281%29.png)

1. Click on "Change leverage" and choose a loop amount.

2. Depending on the loop amount \(ranges between 1 to 10\), your borrow amount, leverage, and liquidation price will be updated accordingly.

{% hint style="danger" %}
Liquidation price increases with loop amount, and a higher liquidation price means you can get liquidated more easily.
{% endhint %}

3. You can adjust the "Swap Tolerance". A lower value means your transaction is more likely to fail e.g. when the exchange rate of MIM token changes during the execution of your transaction.

4. To use a lower gas fee, click on "Update price". Then click "ADD COLLATERAL AND BORROW" and sign the transaction to open a leverage position.

{% hint style="danger" %}
You can add more collateral before your collateral price reaches the liquidation price. When you use leverage, you will forfeit all your collaterals if you get liquidated.
{% endhint %}

