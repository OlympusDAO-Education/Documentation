# Stake Dein OHM \(3, 3\)

Mit Staking können Sie passiv OHM durch Auto-Compounding verdienen. Wenn Sie Ihr OHM bei OlympusDAO staken, erhalten Sie im Gegenzug sOHM \(staked OHM\) im Verhältnis 1:1. Danach erhöht sich Ihr sOHM-Guthaben automatisch in jeder Epoche, basierend auf dem aktuellen APY. 

Sehen Sie sich dieses Video an, um zu erfahren, wie Sie OHM erhalten und auf Olympus staken können:

{% embed url="https://www.youtube.com/watch?v=aXAE1ikVMpM" caption="So erhalten Sie OHM und staken es auf Olympus" %}

## Wie kann man OHM kaufen?

{% hint style="warning" %}
Es gibt mehrere Möglichkeiten, OHM zu kaufen: [Sushiswap](https://app.sushi.com/swap), [Uniswap](https://app.uniswap.org/#/swap) oder DEX-Aggregatoren wie [matcha](https://matcha.xyz/). Achten Sie darauf, **die Slippage zuerst zu überprüfen**, bevor Sie OHM kaufen, da einige eine schlechtere Rate als die anderen aufgrund der geringen Liquidität anbieten.
{% endhint %}

1. Gehen Sie zu der [Sushiswap-Swapseite](https://app.sushi.com/swap?outputCurrency=0x383518188c0c6d7730d91b2c03a03c837814a899). Wir verwenden Sushiswap hier als Beispiel. Es wird empfohlen, den Wechselkurs zwischen verschiedenen DEXen zu vergleichen, um sicherzustellen, dass Sie den besten Preis erhalten.
2. Stellen Sie sicher, dass die Ausgabewährung OHM ist. Sie können auch die Adresse des [OHM-Contract](../contracts/tokens.md#ohm) kopieren und in das Feld für die Ausgabewährung einfügen, um sicherzustellen, dass Sie den richtigen Token tauschen.

![OHM-Contractadresse einf&#xFC;gen](../.gitbook/assets/ohm_contract.png)

1. Sie können eine beliebige Eingabewährung auf der Grundlage Ihres verfügbaren Guthabens wählen. Es wird empfohlen, DAI als Eingabewährung zu verwenden, um den Slippage zu minimieren.

![Stellen Sie sicher, dass die Ausgangsw&#xE4;hrung OHM ist.](../.gitbook/assets/buy_ohm.png)

1. Wählen Sie die Menge an OHM, die Sie eintauschen möchten. Klicken Sie dann auf "Approve" und genehmigen Sie die Transaktion.
2. Nachdem die Transaktion "Genehmigen" erfolgreich bearbeitet wurde, klicken Sie auf "Swap" und unterschreiben die Transaktion.
3. Nach erfolgreicher Swap-Transaktion sollte OHM nun in Ihrem Wallet-Guthaben erscheinen. Wenn Sie es nicht in Ihrer Wallet finden können, fügen Sie die Adresse des [OHM-Contracts](../contracts/tokens.md#ohm) zu Ihrer Wallet hinzu.

{% hint style="info" %}
Die Transaktion "Approve" ist nur erforderlich, wenn Sie OHM zum ersten Mal tauschen; bei späteren Tauschvorgängen müssen Sie nur noch die Transaktion "Swap" durchführen.
{% endhint %}

## Wie Stake ich OHM?

1. Rufen Sie die [Stake Seite auf der OlympusDAO-Website](https://app.olympusdao.finance/#/stake) auf. Wählen Sie die Registerkarte "Stake".
2. Geben Sie in das Eingabefeld den Betrag an OHM ein, den Sie staken möchten. Wenn Sie Ihr gesamtes OHM staken möchten, klicken Sie auf die Schaltfläche "Max" und das Eingabefeld wird mit Ihrem gesamten verfügbaren OHM-Guthaben gefüllt.
3. Klicken Sie auf "Approve" und unterschreiben Sie die Transaktion.
4. Nachdem die Transaktion "Genehmigen" erfolgreich bearbeitet wurde, klicken Sie auf "Stake" und unterschreiben die Transaktion. Voilà, Sie haben Ihr OHM gestaked!

## Wie Unstake ich OHM?

1. Rufen Sie die [Stake Seite auf der OlympusDAO-Website](https://app.olympusdao.finance/#/stake) auf. Wählen Sie die Registerkarte "Unstake".
2. Geben Sie in das Eingabefeld den Betrag an sOHM ein, den Sie unstaken möchten. Wenn Sie Ihr gesamtes sOHM unstaken möchten, klicken Sie auf die Schaltfläche "Max" und das Eingabefeld wird mit Ihrem gesamten verfügbaren sOHM-Guthaben gefüllt.
3. Klicken Sie auf "Approve" und unterschreiben Sie die Transaktion.
4. Nachdem die Transaktion "Genehmigen" erfolgreich bearbeitet wurde, klicken Sie auf "Unstake" und unterschreiben die Transaktion.

_Hinweis: Die Transaktion "Approve" ist nur erforderlich, wenn Sie zum ersten Mal staken/unstaken; bei späteren Stake bzw. Unstake müssen Sie nur noch die Transaktion "Stake" bzw. "Unstake" durchführen._

## Lesen der Informationen

![Die Staking Seite](../.gitbook/assets/staking_page_index.png)

**APY** gibt Ihnen die annualisierte Rendite auf der Grundlage der Rendite an. Sie berücksichtigt den Effekt der Zinseszinsen, da sOHM exponentiell ansteigt.

**TVL** misst den Dollar-Betrag aller abgesicherten OHM in Olympus.

**Current Index** ermöglicht es Ihnen, Ihren Gewinn aus dem staking zu verfolgen. Der Index beginnt bei 1 in Epoche 0 und erhöht sich mit jeder Epoche. Wenn Sie in der Entstehungsphase \(Epoche 0\) gestaked und nie ein OHM unstaked hätten, wäre Ihr Guthaben heute X-mal größer, wobei X der aktuelle Index ist. Sie können den Index verwenden, um Ihre Position zu verfolgen, indem Sie die Indexnummer notieren, wenn Sie staken oder unstaken. Sie teilen die Indexzahl, wenn Sie die Einsätze aufheben, durch die Indexzahl, wenn Sie Einsätze tätigen, um das Verhältnis zu erhalten, um das sich Ihr sOHM-Saldo erhöht hat.

**Your Balance** gibt an, wie viele OHM sich in Ihrem Geldbeutel befinden. Dies ist der Höchstbetrag, den Sie einsetzen können.

**Your Staked Balance** sagt Ihnen, wie viele staked OHM sich in Ihrer Wallet befinden. Dies ist der Höchstbetrag, den Sie aus dem Staking nehmen können.

**Next Rebase** gibt Ihnen die verbleibende Zeit bis zum nächsten Rebase an.

**Reward Yield** gibt an, um wie viel sich Ihr sOHM-Guthaben zu Beginn der nächsten Epoche erhöhen wird. Wenn Sie z.B. 100 OHM einsetzen und die kommende Rebase 0,5427% beträgt, würde Ihr sOHM-Guthaben von 100 auf 100,5427 steigen.

**ROI \(5-Day Rate\)** schätzt, um wie viel sich Ihr sOHM-Guthaben nach 5 Tagen erhöhen wird, wenn die Rendite während dieses Zeitraums gleich bleibt. Wenn Sie z. B. 100 OHM einsetzen und die Rate 8,4577 % beträgt, würde sich Ihr sOHM-Guthaben nach 5 Tagen von 100 auf 108,4577 erhöhen.

