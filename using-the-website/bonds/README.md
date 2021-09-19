# Kaufe einen Bond \(1, 1\)

Bonds ermöglichen es den Nutzern, OHM mit einem Abschlag vom Protokoll zu kaufen, indem sie sie gegen i\) Liquidität \(LP-Token\) oder ii\) andere Vermögenswerte eintauschen. Erstere werden als [Liquiditätsanleihen](../../references/glossary.md#liquidity-bonds) und letztere als [Reserveanleihen](../../references/glossary.md#reserve-bonds) bezeichnet. 

Es dauert etwa 15 Epochen, bis die Anleihen gültig werden, und die OHM-Token werden dem Nutzer in diesem Zeitraum linear zugeteilt. Liquiditätsanleihen helfen dem Protokoll, Liquidität zu akkumulieren und zu binden, während Reserveanleihen es dem Protokoll ermöglichen, seine Schatzkammer und damit seinen RFV schneller zu vergrößern. 

Olympus bietet fünf Arten von Anleihen auf seiner [Website](https://app.olympusdao.finance/#/bonds) an:

* [DAI bond](bond_dai.md)
* [FRAX bond](bond_frax.md)
* [wETH bond](bond_weth.md)
* [OHM-DAI LP bond](ohm-dai-lp-bond.md)
* [OHM-FRAX LP bond](bond_ohm_frax.md)

## Hades

Hades ist eine Funktion, die es Ihnen ermöglicht, Bonds zu kaufen und die erworbenen OHM an eine andere Adresse zu senden. Dies ist nützlich für zusätzliche Privatsphäre oder für den Kauf mehrerer Bonds, während die aktuellen Bonds noch gültig sind. Beachten Sie, dass bei mehreren Bonds auf demselben Konto die ausstehenden Belohnungen der früheren Bonds verfallen.

1. Gehen Sie zur [Bond Seite ](https://app.olympusdao.finance/#/bonds)und wählen Sie die Art des Bonds, die Sie kaufen möchten.
2. Wählen Sie den Betrag, den Sie bonden möchten, und klicken Sie dann auf das Zahnradsymbol oben rechts auf der Seite.

   ![](../../.gitbook/assets/cogwheel.png)

3. Das Hades-Menü wird eingeblendet. Im Feld Empfängeradresse können Sie eine andere Adresse angeben, an die das vested OHM gesendet werden soll. Standardmäßig ist das Feld mit Ihrer aktuellen Adresse gefüllt.

   ![](../../.gitbook/assets/hades.png)

4. Sie können auch das Feld "Slippage" ändern, um die Wahrscheinlichkeit zu erhöhen oder zu verringern, dass Ihr Auftrag ausgeführt wird. Eine höhere Slippage erhöht diese Wahrscheinlichkeit, aber Sie erhalten möglicherweise einen unerwünschten Füllpreis.
5. Schließen Sie das Hades-Menü, indem Sie erneut auf das Zahnradsymbol klicken.
6. Klicken Sie auf "Approve und unterschreiben Sie die Transaktion.
7. Nachdem die Transaktion "Approve" erfolgreich bearbeitet wurde, klicken Sie auf "Bond" und unterschreiben die Transaktion. Voila, Sie haben Ihre erste Anleihe mit Hades gekauft!

_Hinweise:_

* _Die Transaktion "Approve" ist nur bei dem ersten Bond erforderlich; bei späteren Bonds müssen Sie nur noch die Transaktion "Bond" durchführen._
* _Wenn Sie den Hades verwenden, dürfen Sie den Betrag des Bonds nicht mehr ändern, nachdem Sie das Hades-Menü geschlossen haben, da sonst die Empfängeradresse zurückgesetzt wird._

## **How to Redeem**

Go to [Bond page](https://app.olympusdao.finance/#/bonds) and select the bond type you have purchased. Select the "Redeem" tab. Then, click "Claim Rewards" to claim all of your available rewards.

## Reading the Info

![](../../.gitbook/assets/modal.png)

**Balance** is your balance of SLP tokens. This is the asset used to create a bond.

**Bond Price** is the price of OHM you get from bonding. You can calculate the bond price using the following formulae:

* SLP Bond: \(Value of your SLP token / OHM you'll get from bonding\)
* DAI Bond: \(Value of your DAI token / OHM you'll get from bonding\)

**Market Price** is the market price of OHM.

**You Will Get** tells you how many OHM you will get from bonding.

**Debt Ratio** measures the total amount of OHM created from bonds that have yet to be paid out by the protocol. The debt ratio is calculated differently for SLP bond and DAI bond:

* SLP Bond: \(OHM created from unredeemed bonds / OHM total supply\)
* DAI Bond: \(OHM created from unredeemed bonds / OHM circulating supply\)

**Vesting Term** measures the period a bond takes to fully redeem. This number is in Ethereum blocks. 33110 blocks is approximately 5 days or 15 epochs.

**Discount** is the difference between the bond price and the market price. In the screenshot above, bonding would give you a 10.63% discount versus buying the same amount of OHM from the market.

![](../../.gitbook/assets/modal_redeem.png)

**Pending Rewards** is the amount of OHM you are entitled to receive from bonding.

**Claimable Rewards** is the amount of OHM that you can claim now. This amount keeps increasing as OHM is vested to you over the bonding period.

**Full Bond Maturation** refers to the Ethereum block when the bond is fully redeemable.

