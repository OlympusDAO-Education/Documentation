# FAQ

## Wozu brauchen wir überhaupt Olympus?

An den Dollar gebundene Stablecoins sind eine unverzichtbare Variante von Kryptowährungen, da sie im Vergleich zu Token wie Bitcoin und Ether nur geringe Preisschwankungen aufweisen. Nutzer setzen sie häufig für Transaktionen ein, da sie der Meinung sind, dass die Stablecoins morgen die gleiche Kaufkraft besitzen werden wie heute. Doch dabei handelt es sich um einen Trugschluss. Der Dollar wird von der US-Bundesregierung und deren Zentralbank kontrolliert. Daher bewirkt eine Abwertung des Dollars auch eine Abwertung der Stablecoins.

OlympusDAO versucht, dieses Problem durch eine ungebundene Stablecoin namens OHM zu lösen. Indem der Schwerpunkt auf dem Bestandswachstum und weniger auf der Wertsteigerung liegt, hofft OlympusDAO, dass OHM als Währung seine Kaufkraft behält, unabhängig von Schwankungen am Markt.

## Ist OHM eine Stablecoin?

Nein, OHM ist keine Stablecoin. Ohm soll eine algorithmische Reserve-Währung sein, die von anderen dezentralisierten Assets gestützt wird. Ähnlich wie bei der Idee des Goldstandards bietet OHM einen frei beweglichen Grundwert, auf den seine Besitzer stets zurückgreifen können, ganz einfach aufgrund der anteiligen Reserven im Olympus-Vermögen, auf denen der intrinsische Wert von OHM beruht.

## Ist OHM gestützt oder gebunden?

Jedes OHM wird von 1 DAI gestützt, ist aber nicht daran gebunden. Weil das Olympus-Protokoll für jedes OHM mindestens 1 DAI in seinem Vermögen hält, kann es OHM zurückkaufen und vernichten, sobald der Kurs unter 1 DAI sinkt. Dies bewirkt, dass der Preis für OHM wieder auf 1 DAI gehoben wird. Der Kurs von OHM kann allerdings jederzeit über 1 DAI steigen, da das Protokoll keine Obergrenze vorgibt. Einfach ausgedrückt bedeutet gebunden == 1, gestützt hingegen >= 1.

Man könnte auch sagen, der Mindestpreis oder intrinsische Wert von OHM ist 1 DAI. Wir glauben, dass der tatsächliche Preis immer 1 DAI + ein bestimmter Aufpreis sein wird, doch das wird der Markt entscheiden.

## Wie funktioniert das Ganze?

Grundsätzlich setzt sich OlympusDAO zusammen aus dem vom Protokoll verwalteten Vermögen, der Protokoll-eigenen Liquidität (Protocol Owned Liquidity, [POL](../references/glossary.md#pol)), den Bond-Mechanismen und den Vergütungen für das Staking, die auf die Vergrößerung des OHM-Bestands ausgelegt sind.

Die Verkäufe von Bonds führen zu Einnahmen, die das Protokoll nutzt, um OHM zu prägen und an die Staker auszuschütten. Durch [Liquiditäts-Anleihen](../references/glossary.md#liquidity-bonds) kann das Protokoll eigene Liquidität anhäufen. Der Punkt "[Warum ist POL wichtig?](basics.md#why-is-pol-important)" erklärt das weiter unten noch genauer.

## Was hat es mit (3,3) und (1,1) auf sich?

(3,3) veranschaulicht die Idee, dass ein kooperatves Verhalten aller Teilnehmer den größtmöglichen Gewinn für alle Beteiligten erzeugt (aus spieltheoretischer Sicht). Derzeit gibt es drei Möglichkeiten, wie sich ein Teilnehmer verhalten kann:

* Staken (+2)
* Bonden (+1)
* Verkaufen (-2)

Staken und Bonden sind vorteilhaft für das Protokoll, während Verkaufen als nachteilig gilt. Staken und Verkaufen beeinflusst außerdem den Preis, während Bonden keine Auswirkung darauf hat (wir nehmen an, dass OHM zunächst auf dem Markt gekauft wird, bevor es gestaked werden kann, daher der Einfluss auf den Preis). Sind im Fall von zwei Akteuren beide Aktionen vorteilhaft, dann erhält jeder, der für eine Preisbewegung sorgt, auch die Hälfte des Nutzens (+1). Sind die Aktionen gegenläufig, erhält der schädliche Akteur die Hälfte des Gewinns (+1) und der hilfreiche Akteur trägt die Hälfte des Verlustes (-1). Wenn beide Aktionen nachteilig sind, also beide Akteure verkaufen, trägt jeder die Hälfte des Verlustes (-1).

Für zwei Akteure ergibt sich daraus folgendes Schema, das zeigt, welche Möglichkeiten beide haben und welche Folgen dies jeweils hat:

![](../.gitbook/assets/game\_theory.png)

* Wenn beide staken (3, 3), dann ist das am besten sowohl für die Akteure als auch für das Protokoll (3 + 3 = 6).
* Wenn einer von beiden staked und der andere bondet, dann ist das auch gut, denn Staken nimmt OHM vom Markt und hinterlegt es im Protokoll, während Bonden dem Olympus-Vermögen Liquidität und DAI beschert (3 + 1 = 4).
* Wenn einer von beiden verkauft, dann mindert es die positiven Auswirkungen des anderen, der staked oder bondet (1 - 1 = 0).
* Wenn beide verkaufen, hat das die schlechtesten Auswirkungen, sowohl für die Akteure als auch für das Protokoll (-3 - 3 = -6).

## Warum ist PCV wichtig?

Protocol Controlled Value (PCV) ist die Menge an Assets, die das Olympus-Vermögen besitzt und kontrolliert. Da das Protokoll die Werte in seinem Vermögen besitzt, kann OHM nur vom Protokoll geprägt oder vernichtet werden. Das stellt auch sicher, dass das Protokoll für 1 OHM stets 1 DAI garantieren kann. Das Risiko einer Investition ist daher einfach abzuschätzen, da jeder sicher sein kann, dass das Protokoll OHM, das unter 1 DAI fällt, mit Mitteln aus seinem Vermögen so lange zurückkaufen wird, bis keines mehr übrig ist. Man muss nicht notwendigerweise der Zentralbank vertrauen, aber man kann sich immer auf den Programmcode verlassen.

Indem das Protokoll mehr PCV anhäuft, kann es eine längere Zeitspanne an Ausschüttungen garantieren. Die Staker können daher sicher sein, dass die gegenwärtige Zinsrate für das Staken länger aufrecht erhalten werden kann, weil das Olympus-Vermögen über mehr Werte verfügt.

## Warum ist POL wichtig?

Protokoll-eigene Liquidität (Protocol Owned Liquidity, POL) ist die Menge an LP(Liquiditäts-Provider)-Token (z.B. OHM-DAI LP-Bonds) im Olympus-Vermögen. Dank des Anleihe-Mechanismus ist Olympus [Eigentümer des größten Teils seiner Liquidität](https://dune.xyz/shadow/Olympus-\(OHM\)). Das hat mehrere Vorteile:

* Olympus muss keine hohen Farming-Zinsen ausschütten, um Liquidität von Geldgebern anzulocken, sprich Liquidität zu mieten.
* Olympus garantiert dem Markt, dass stets Liquidität vorhanden ist, um Kauf- oder Verkaufs-Transaktionen zu ermöglichen.
* Als größter Liquiditäts-Provider (LP) verdient Olympus den Löwenanteil der LP-Gebühren, eine weitere Einkommensquelle für das Gemeinschaftsvermögen.
* Die gesamte POL kann genutzt werden, um OHM zu stützen. Die LP-Token werden dazu mit ihrem Risiko-freien Wert (RFV, Risk Free Value), sprich dem garantierten Kapital angesetzt. Mehr über die Beweggründe dazu findet sich in diesem [Medium-Artikel](https://olympusdao.medium.com/dai-bonds-a-more-effective-sales-mechanism-c9a57586f1f7).

## Was würde im Fall eines Kassenansturms bei Olympus passieren?

Bankensysteme mit Mindestreserven funktionieren, weil nicht alle Anleger gleichzeitig ihr Geld abheben. Das Vertrauen eines Anlegers in das Bankensystem beruht auf Reglementierung und auf Sicherungssystemen wie der Federal Deposit Insurance Corporation (FDIC), der Bundeseinlagenversicherungsgesellschaft der USA.

OHM hat zwar keine Einlagensicherung, aber dafür ein Anreizsystem, das Staker schützt. Ein Blick auf einen hypothetischen Ansturm auf die Bank soll zeigen, wie das funktioniert. Für dieses Szenario nehmen wir an, dass die Mehrzahl der Staker in Panik gerät und ihre Token auf Olympus unstaken wird, also abhebt. Der Anteil an gestaktem OHM fällt von 92% abrupt auf 3,3%, und es bleiben nur 55.000 OHM gestaked.

Außerdem nehmen wir an, dass Zuflüsse an garantiertem Kapital (RFV, Risk Free Value) in das Protokoll-Vermögen komplett versiegen. Um einen Vergleich zu nennen: Derzeit wächst das RFV um [etwa 1 Million US$ alle zwei Tage](https://dune.xyz/queries/29153/58862). Während eines Kassensturms würde dies allerdings sehr wahrscheinlich aufhören.

Schließlich nehmen wir weiter an, dass die letzten verbleibenden Staker zu einem Preis von 500 US$ pro OHM eingekauft haben. Die Anfangsinvestition dieser Staker wäre dann:

$$
\$500/OHM * 55.000\ OHM = \$27,5\ Millionen
$$

Am 15. September 2021 betrug der gesamte Bestand an OHM 2.082.553 und das RFV 47.041.833 US$. Erinnern wir uns daran, dass für jedes 1 OHM stets 1 US$ hinterlegt ist (in Form von DAI oder FRAX). Ziehen wir die beiden vorstehenden Zahlen voneinander ab, erhalten wir einen Wert von 44.959.280 OHM, die früher oder später an die verbleibenden Staker ausgeschüttet werden. In etwa einem Jahr werden diese Staker, die derzeit 55.000 OHM halten, folgende Menge besitzen:

$$
55.000 + 44.959.280 = 45.014.280\ OHM
$$

Wenn sie weiter staken, verwandelt sich eine Anfangsinvestition von 27,5 Millionen US$ in ein Vermögen von etwa 45 Millionen US$, allein aufgrund des Cash Flows (denn 1 OHM ist jederzeit von 1 US$ gestützt). In diesem Szenario eines hypothetischen Kassensturms bekommen die Staker, die ihre Position halten, nicht nur ihr Geld zurück, sondern machen auch noch Gewinn. Aus diesem Grund ist [(3,3)](basics.md#what-is-the-deal-with-3-3-and-1-1) nicht nur ein beliebtes Meme, sondern tatsächlich die am weitesten verbreitete OHM-Strategie

Es ist sehr unwahrscheinlich, dass sich das obige Szenario tatsächlich so abspielt, denn sobald andere Investoren merken, dass die verbleibenden Staker extrem hohe Gewinne machen, werden sie die Strategie imitieren und OHM kaufen und staken. Das ist auch der Grund, warum der Anteil an gestaktem OHM seit dem Launch konstant über 90% lag.

Anmerkung: Die meisten Daten in obigem Beispiel stammen von [dieser Dune Analytics Seite](https://duneanalytics.com/shadow/Olympus-\(OHM\)).

## Why is the market price of OHM so volatile?

It is extremely important to understand how early in development the OlympusDAO protocol is. A large amount of discussion has centered around the current price and expected a stable value moving forward. The reality is that these characteristics are not yet determined. The network is currently tuned for expansion of OHM supply, which when paired with the staking, bonding, and yield mechanics of OlympusDAO, result in a fair amount of volatility.

OHM could trade at a very high price because the market is ready to pay a hefty premium to capture a percentage of the current market capitalization. However, the price of OHM could also drop to a large degree if the market sentiment turns bearish. We would expect significant price volatility during our growth phase so please **do your own research** whether this project suits your goals.

## What is the point of buying it now when OHM trades at a very high premium?

When you buy and stake OHM, you capture a percentage of the supply (market cap) which will remain close to a constant. This is because your staked OHM balance also increases along with the circulating supply. The implication is that if you buy OHM when the market cap is low, you would be capturing a larger percentage of the market cap.

## What is a rebase?

Rebase is a mechanism by which your staked OHM balance increases automatically. When new OHM are minted by the protocol, a large portion of it goes to the stakers. Because stakers only see staked OHM balance instead of OHM, the protocol utilizes the rebase mechanism to increase the staked OHM balance so that 1 staked OHM is always redeemable for 1 OHM.

## What is reward yield?

Reward yield is the percentage by which your staked OHM balance increases on the next epoch. It is also known as _rebase rate_. You can find this number on the [Olympus staking page](https://app.olympusdao.finance/#/stake).

## What is APY?

APY stands for annual percentage yield. It measures the real rate of return on your principal by taking into account the effect of compounding interest. In the case of OlympusDAO, your staked OHM represents your principal, and the compound interest is added periodically on every epoch (2200 Ethereum blocks, or around 8 hours) thanks to the rebase mechanism.

One interesting fact about APY is that your balance will grow not linearly but exponentially over time! Assuming a daily compound interest of 2%, if you start with a balance of 1 OHM on day 1, after a year, your balance will grow to about 1377. That is a lot!

![The power of compounding](../.gitbook/assets/apy.png)

## How is the APY calculated?

The APY is calculated from the reward yield (a.k.a rebase rate) using the following equation:

$$
APY = ( 1 + rewardYield )^{1095}
$$

It raises to the power of 1095 because a rebase happens 3 times daily. Consider there are 365 days in a year, this would give a rebase frequency of 365 \* 3 = 1095.

Reward yield is determined by the following equation:

$$
rewardYield = OHM_{distributed} / OHM_{totalStaked}
$$

The number of OHM distributed to the staking contract is calculated from OHM total supply using the following equation:

$$
OHM_{distributed} = OHM_{totalSupply} \times rewardRate
$$

Note that the reward rate is subject to change by the protocol. For example, it has been revised due to [this latest proposal](https://forum.olympusdao.finance/d/77-oip-18-reward-rate-framework-and-reduction).

## Why does the price of OHM become irrelevant in long term?

As illustrated above, your OHM balance will grow exponentially over time thanks to the power of compounding. Let's say you buy an OHM for $400 now and the market decides that in 1 year time, the intrinsic value of OHM will be $2. Assuming a daily compound interest rate of 2%, your balance would grow to about 1377 OHMs by the end of the year, which is worth around $2754. That is a cool $2354 profit! By now, you should understand that you are paying a premium for OHM now in exchange for a long-term benefit. Thus, you should have a long time horizon to allow your OHM balance to grow exponentially and make this a worthwhile investment.

## What will be OHM's intrinsic value in the future?

There is no clear answer for this, but the intrinsic value can be determined by the treasury performance. For example, if the treasury could guarantee to back every OHM with 100 DAI, the intrinsic value will be 100 DAI. It can also be decided by the DAO. For example, if the DAO decides to [raise the price floor of OHM](https://forum.olympusdao.finance/d/31-use-price-floor-as-tool-for-monetary-policy), its intrinsic value will rise accordingly.

## How does the protocol manage to maintain the high staking APY?

Let’s say the protocol targets an APY of 100,000%. This would translate to a rebase rate of about 0.6328%, or a daily growth of about 2%. Please refer to the equation above to learn [how APY is calculated from the rebase rate](basics.md#how-is-the-apy-calculated).

If there are 100,000 of OHM staked right now, the protocol would need to mint an additional 2000 OHM to achieve this daily growth. This is achievable if the protocol can bring in at least 2000 DAI daily from bond sales. If the protocol fails to achieve this, the APY of 100,000% cannot be guaranteed.

## Do I have to unstake and stake OHM on every epoch to get my rebase rewards?

No. Once you have staked OHM with OlympusDAO, your staked OHM balance will auto-compound on every epoch. That increase in balance represents your rebase rewards.

## How do I track my rebase rewards?

You can track your rebase rewards by calculating the increase in your staked OHM balance.

1. Record down the Current Index value on the [staking page](https://app.olympusdao.finance/#/) when you first stake your OHM. Let's call this the Start Index.

![](../.gitbook/assets/index\_old.png)

1. After staking for some time, if you want to determine by how much your balance has increased, check the Current Index value again. Let's call this the End Index.

![](../.gitbook/assets/index\_new.png)

1. By dividing the End Index by Start Index, you would get the ratio by which your staked OHM balance has increased.

$$
ratio = endIndex / startIndex
$$

1. In this example, the OHM balance has grown by 1.5 times.

$$
ratio = 13.2\ /\ 8.8\newline = 1.5
$$
