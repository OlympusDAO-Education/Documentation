# OHM staken (3, 3)

Beim Staken erwirtschaftet OHM passiv Erträge durch die automatische Verzinsung. Wer OHM bei OlympusDAO staked, erhält dafür sOHM (staked OHM) im Verhältnis 1:1. Dieses sOHM-Guthaben erhöht sich automatisch nach jeder Epoche basierend auf der aktuellen jährlichen Ertragsrate (Annual Percentage Yield, APY).

Dieses Video erklärt, wie man OHM erwerben und auf Olympus staken kann:

{% embed url="https://www.youtube.com/watch?v=aXAE1ikVMpM" %}
So kommt man an OHM und staked es bei Olympus
{% endembed %}

## OHM kaufen

{% hint style="warning" %}
Es gibt mehrere Möglichkeiten, OHM zu kaufen: [Sushiswap](https://app.sushi.com/swap), [Uniswap](https://app.uniswap.org/#/swap), oder DEX-Aggregatoren wie [matcha](https://matcha.xyz). Wichtig ist es, vor dem Kauf von OHM die **Slippage zu beachten**, da manche Plattformen aufgrund geringer Liquidität schlechtere Kurse bieten.
{% endhint %}

1. Gehen Sie zu [dieser Sushiswap Swap-Seite](https://app.sushi.com/swap?outputCurrency=0x383518188c0c6d7730d91b2c03a03c837814a899). Wir nutzen SushiSwap als ein Beispiel. Es empfiehlt sich, die Tauschkurse auf mehreren DEX-Plattformen zu vergleichen, um den besten Preis ausfindig zu machen.
2. Stellen Sie sicher, dass die Zielwährung OHM ist. Sie können auch die [OHM-Vertragsadresse](../contracts/tokens.md#ohm) kopieren und ins Feld für die Zielwährung einfügen, um sicher zu sein, dass sie in den richtigen Token umtauschen.

![OHM-Vertragsadresse einfügen](../.gitbook/assets/ohm\_contract.png)

* 3\. Sie können eine beliebige Ausgangswährung einstellen, je nach verfügbarem Guthaben in Ihrer Wallet. Empfehlenswert ist DAI als Ausgangswährung, um die Slippage möglichst gering zu halten.

![Make sure the output currency is OHM](../.gitbook/assets/buy\_ohm.png)

4\. Geben Sie den Betrag an OHM ein, in den Sie tauschen möchten. Dann klicken Sie auf "Genehmigen" und unterzeichnen die Transaktion in Ihrer Wallet.

5\. Sobald die Genehmigung erfolgreich war, klicken Sie auf "Swap" und unterzeichnen Sie erneut.

6\. Wenn die Swap-Transaktion erfolgreich war, sollten Sie die OHM in Ihrer Wallet sehen. Falls nicht, fügen Sie die OHM-Vertragsadresse manuell zu Ihrer Wallet hinzu.

{% hint style="info" %}
Die "Genehmigungs"-Transaktion ist nur nötig, wenn Sie zum ersten Mal OHM swappen. Zukünftiger Umtausch erfordert nur die "Swap"-Transaktion.
{% endhint %}

## OHM staken

1. Gehen Sie zum [Stake-Bereich der OlympusDAO Webseite](https://app.olympusdao.finance/#/). Wählen Sie "Stake".
2. Falls Sie zum ersten Mal staken, erteilen Sie zunächst die Genehmigung, indem Sie auf "Approve" klicken und unterzeichnen.
3. Geben Sie die gewünschte Menge an OHM an, die Sie staken wollen. Falls Sie alles OHM staken möchten, können Sie auf "Max." klicken, und der verfügbare Höchstbetrag erscheint automatisch im Eingabefeld.
4. Klicken Sie auf "Staken" und unterzeichnen Sie die Transaktion. Voila, Sie haben OHM gestaked!

## OHM unstaken

1. Gehen Sie zum [Stake-Bereich der OlympusDAO Webseite](https://app.olympusdao.finance/#/). Wählen Sie "Unstake".
2. Falls Sie zum ersten Mal unstaken, erteilen Sie zunächst die Genehmigung, indem Sie auf "Approve" klicken und unterzeichnen.
3. Geben Sie die gewünschte Menge an OHM an, die Sie unstaken wollen. Falls Sie alles OHM unstaken möchten, können Sie auf "Max." klicken, und der verfügbare Höchstbetrag erscheint automatisch im Eingabefeld.
4. Klicken Sie auf "Unstaken" und unterzeichnen Sie die Transaktion.

_Hinweis: Die "Genehmigungs"-Transaktion wird nur benötigt, wenn Sie zum ersten Mal staken oder unstaken. Nachfolgende Transaktionen erfondern nur noch "Staken" oder "Unstaken"._

## Angaben auf der Staking-Seite

![The staking page](../.gitbook/assets/staking\_page\_index.png)

**APY:** Die jährliche Ertragsrate (Annual Percentage Yield, APY) gibt die tatsächliche Zinsrate an. Sie berücksichtigt die Zinseszinsen über den Zeitraum von einem Jahr, da die Ausschüttungen von sOHM exponentiell wachsen.

**TVL:** Das angelegte Gesamtvermögen (Total Value Locked, TVL) ist der Wert aller gestaketen OHM in US-Dollar.

**Current Index:** Der aktuelle Index ermöglicht es, die Ertragsentwicklung durch Staken zu verfolgen. Der Index startet bei Epoche 0 mit dem Wert 1 und erhöht sich in jeder weiteren Epoche. Wenn Sie OHM zum Zeitpunkt der Genesis gestaked haben und bisher nichts davon unstaked wurde, wäre Ihr Guthaben heute X-mal größer, wobei X der Wert des Current Index ist. Der Index lässt sich nutzen, um die Wertentwicklung einer gestaketen Position zu verfolgen: Dazu notiert man sich den Wert des Index sowohl beim Staken als auch beim Unstaken. Teilt man letzteren durch ersteren Wert ergibt sich der Faktor, um den sich das sOHM-Guthaben vermehrt hat.

**Ihr Guthaben:** die Menge an ungestaketem OHM in Ihrer Wallet. Dies ist der Höchstbetrag, den Sie staken können.

**Ihr gestaketes Guthaben:** die Menge an gestaketem OHM in Ihrer Wallet. Dies ist der Höchstbetrag, den Sie unstaken können.

**Nächste Ausschüttung:** die verbleibende Zeit bis zur nächsten Ausschüttungsrunde.

**Reward Yield:** Der Belohnungsertrag nennt die konkrete Menge an sOHM, um die Ihr Guthaben zu Beginn der nächsten Epoche ansteigen wird. Wenn Sie beispielsweise 100 OHM staken und die Ausschüttungsrate 0,5427% beträgt, dann wird Ihr Guthaben an sOHM von 100 auf 100, 5427 ansteigen.

**ROI (5-Tages-Rate):** Dieser Wert gibt an, um wie viel Ihr sOHM-Guthaben in den nächsten 5 Tagen ansteigt, wenn der Belohnungsertrag während dieser Zeit gleich bleibt. Wenn Sie beispielsweise 100 OHM staken und die Ausschüttungsrate 8,4577% beträgt, dann wird Ihr Guthaben an sOHM nach 5 Tagen von 100 auf 108,4577 ansteigen.
