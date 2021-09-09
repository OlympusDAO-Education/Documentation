# FAQ

## Warum brauchen wir überhaupt OlympusDAO?

An den Dollar gekoppelte Stablecoins sind aufgrund ihrer geringen Volatilität im Vergleich zu Token wie Bitcoin und Ether zu einem wesentlichen Bestandteil der Kryptowährung geworden. Die Nutzer fühlen sich bei Transaktionen mit Stablecoins wohl, weil sie wissen, dass sie heute die gleiche Kaufkraft besitzen wie morgen. Doch das ist ein Trugschluss. Der Dollar wird von der US-Regierung und der Federal Reserve kontrolliert. Das bedeutet, dass eine Abwertung des Dollars auch eine Abwertung dieser Stablecoins bedeutet.

OlympusDAO möchte dieses Problem lösen, indem es einen stabilen, nicht an den Kurs gebundenen Coin namens OHM schafft. OlympusDAO hofft, dass OHM als eine Währung fungieren kann, die ihre Kaufkraft unabhängig von der Marktvolatilität halten kann, indem sie sich auf das Wachstum des Angebots und nicht auf den Preisanstieg konzentriert.

## Ist OHM eine stable coin?

Nein, OHM ist keine stable coin. Vielmehr strebt OHM danach, eine algorithmische Reservewährung zu werden, die von anderen dezentralen Vermögenswerten gestützt wird. Ähnlich der Idee des Goldstandards bietet OHM einen frei schwankenden Wert, auf den seine Nutzer immer zurückgreifen können, einfach aufgrund der fraktionierten Schatzreserven, aus denen OHM seinen inneren Wert bezieht.

## OHM wird gesichert, nicht gekoppelt.

Jedes OHM ist mit 1 DAI unterlegt, nicht daran gekoppelt. Da das Schatzamt jedes OHM mit mindestens 1 DAI unterlegt, würde das Protokoll OHM zurückkaufen und verbrennen, wenn sie unter 1 DAI gehandelt werden. Dies hat zur Folge, dass der OHM-Preis wieder auf 1 DAI steigt. OHM könnte immer über 1 DAI gehandelt werden, da es keine vom Protokoll auferlegte Obergrenze gibt. Man kann sich vorstellen, dass pegged == 1 ist, während backed &gt;= 1 ist. Man könnte sagen, dass der Mindestpreis oder der innere Wert des OHM bei 1 DAI liegt. 

Wir sind der Meinung, dass der tatsächliche Preis immer 1 DAI + Aufschlag betragen wird, aber das muss letztendlich der Markt entscheiden.

## Wie funktioniert das?

Im Großen und Ganzen besteht OlympusDAO aus einer vom Protokoll verwalteten Schatzkammer, protokolleigener Liquidität, einem Bond-Mechanismus und hohen Staking-Belohnungen, die dazu dienen, die Angebotsausweitung zu kontrollieren. 

Die Anleihe generiert Gewinn für das Protokoll, und die Schatzkammer verwendet den Gewinn, um OHM zu prägen und sie an die Staker zu verteilen. Mit der LP-Anleihe ist das Protokoll in der Lage, Liquidität zu akkumulieren, um die Stabilität des Systems zu gewährleisten.

## Was hat es mit \(3,3\) und \(1,1\) auf sich?

\(3,3\) ist die Idee, dass, wenn alle in Olympus kooperieren, dies den größten Gewinn für alle bringen würde \(vom Standpunkt der [Spieltheorie](https://en.wikipedia.org/wiki/Game_theory) aus gesehen\). Derzeit gibt es drei Aktionen, die ein Nutzer durchführen kann:

* Staking \(+2\)
* Bonding \(+1\)
* Verkauf \(-2\)

Der Staking und die Bonding gelten als vorteilhaft für das Protokoll, während der Verkauf als nachteilig angesehen wird. Staking und Verkäufe führen auch zu einer Preisveränderung, während das Bonding dies nicht tut \(wir betrachten den Kauf von OHM auf dem Markt als Voraussetzung für Einsätze, wodurch eine Preisveränderung verursacht wird\). Wenn beide Aktionen vorteilhaft sind, erhält der Akteur, der den Preis bewegt, auch die Hälfte des Vorteils \(+1\). Wenn beide Handlungen gegensätzlich sind, erhält der schlechte Akteur, der den Preis bewegt, die Hälfte des Nutzens \(+1\), während der gute Akteur, der den Preis bewegt, die Hälfte des Nachteils \(-1\) erhält. Wenn beide Handlungen nachteilig sind, was bedeutet, dass beide Akteure verkaufen, erhalten sie beide die Hälfte des Nachteils \(-1\).

Bei zwei Akteuren werden also alle Szenarien, was sie tun könnten, und die Auswirkungen auf das Protokoll hier dargestellt:

![](../.gitbook/assets/game_theory.png)

* Wenn wir beide auf \(3, 3\) setzen, ist das das Beste für uns beide und das Protokoll \(3 + 3 = 6\).
* Wenn einer von uns einen Stake macht und der andere einen Bond, ist das auch gut, denn der Einsatz nimmt OHM vom Markt und steckt sie in das Protokoll, während die Bond-Liquidität und DAI für die Staatskasse liefert \(3 + 1 = 4\).
* Wenn einer von uns verkauft, verringert sich der Aufwand des anderen, der den Stake oder den Bond tätigt \(1 - 1 = 0\).
* Wenn wir beide verkaufen, ist das Ergebnis für uns beide und das Protokoll am schlechtesten \(-3 - 3 = -6\).

## Warum ist PCV wichtig?

Da das Protokoll die Mittel in seiner Schatzkammer kontrolliert, können OHM nur vom Protokoll geprägt oder verbrannt werden. Dies garantiert auch, dass das Protokoll immer 1 OHM mit 1 DAI zurückzahlen kann. Sie können das Risiko Ihrer Investition leicht definieren, da Sie darauf vertrauen können, dass das Protokoll unbegrenzt OHM unter 1 DAI mit den Mitteln des Schatzamtes kaufen wird, bis niemand mehr zum Verkauf übrig ist. Sie können der FED nicht vertrauen, aber Sie können dem Code vertrauen.

Je mehr PCV das Protokoll anhäuft, desto mehr Runway ist für die Staker garantiert. Dies bedeutet, dass die Staker darauf vertrauen können, dass der aktuelle APY für einen längeren Zeitraum aufrechterhalten werden kann, da mehr Mittel in der Kasse vorhanden sind.

## Was wird passieren, wenn es einen Banküberfall auf Olympus gibt?

Das fraktionierte Mindestreserve-Bankwesen funktioniert, weil die Einleger ihr Geld nicht auf einmal abheben. Das Vertrauen der Einleger in das Bankensystem beruht auf Vorschriften und Einrichtungen wie der Federal Deposit Insurance Corporation \(FDIC\).

Das OHM verfügt nicht über eine FDIC-Versicherung, aber es hat eine Anreizstruktur, die die Anleger schützt. Schauen wir uns an, wie es sich bei einem hypothetischen Bank-Run verhält. In diesem Szenario gehen wir davon aus, dass die Mehrheit der Staker in Panik gerät und ihre Token von Olympus abzieht - der Prozentsatz der Staker, der jetzt bei 92 % liegt, bricht schnell auf 3,3 % ein, so dass nur noch 20.000 OHM im Einsatz sind.

Als nächstes nehmen wir an, dass die Zuflüsse des risikofreien Werts \(RFV\) in das Schatzamt vollständig versiegen. Zum Vergleich: Der RFV wächst derzeit alle 3 Tage um etwa 1 Million Dollar. Während eines Bank-Runs wird dieses Wachstum jedoch wahrscheinlich aufhören.

Schließlich gehen wir davon aus, dass diese letzten Staker zu einem Preis von 500 $ pro OHM einsteigen. Die Anfangsinvestition dieser Staker wäre dann:

$$
\$500/OHM * 20,000\ OHM = \$10\ million
$$

Mit Stand vom 12. Juli 2021 beträgt der Gesamtbestand an OHM 734.421 und der RFV 13.905.970 $. Zur Erinnerung: 1 OHM ist durch 1 USD \(DAI oder FRAX\) gedeckt. Durch Subtraktion dieser beiden Zahlen wissen wir, dass letztendlich 13.171.549 OHM an die verbleibenden Staker ausgegeben werden. In etwa einem Jahr werden diese Staker, die 20.000 OHM halten, über:

$$
20,000 + 13,171,549 = 13,191,549\ OHM
$$

Aus den 10 Millionen Dollar, die diese Staker investiert haben, werden allein durch den Cashflow etwa 13,2 Millionen Dollar, wenn sie ihre Einsätze beibehalten \(zur Erinnerung: 1 OHM ist durch 1 USD gedeckt\). In diesem Bank-Run-Szenario erhalten die Staker, die ihre Einsätze beibehalten, nicht nur ihr Geld zurück, sondern machen auch einen gewissen Gewinn. Daher ist [\(3,3\)](basics.md#was-hat-es-mit-3-3-und-1-1-auf-sich) nicht nur ein beliebtes Mem, sondern tatsächlich eine dominante Strategie.

Es ist unwahrscheinlich, dass das obige Szenario eintritt, denn wenn andere Leute herausfinden, dass extrem hohe Belohnungen an die Staker gezahlt werden, werden sie die Strategie kopieren, indem sie OHM kaufen und einsetzen. Das ist auch der Grund, warum der Prozentsatz der OHM, die in Olympus eingesetzt werden, seit dem Start konstant über 90 % liegt.

_Hinweis: Die meisten der oben genannten Daten stammen von dieser_ [_Dune Analytics-Seite_](https://dune.xyz/shadow/Olympus-%28OHM%29)_._

## Warum ist der Marktpreis des OHM so volatil?

Es ist äußerst wichtig zu verstehen, wie früh sich das OlympusDAO-Protokoll in der Entwicklung befindet. Ein großer Teil der Diskussion drehte sich um den aktuellen Preis und die Erwartung eines stabilen Wertes in der Zukunft. Die Realität ist, dass diese Eigenschaften noch nicht festgelegt sind. Das Netzwerk ist derzeit auf die Ausweitung des OHM-Angebots eingestellt, was in Verbindung mit dem Staking-, Bonding- und Yield-Mechanismus von OlympusDAO zu einer gewissen Volatilität führt.

OHM könnte zu einem sehr hohen Preis gehandelt werden, weil der Markt bereit ist, einen kräftigen Aufschlag zu zahlen, um einen Prozentsatz der aktuellen Marktkapitalisierung zu erhalten. Der Kurs von OHM könnte aber auch stark fallen, wenn sich die Marktstimmung ins Negative wendet. Wir erwarten während unserer Wachstumsphase erhebliche Kursschwankungen. Bitte **prüfen Sie daher selbst**, ob dieses Projekt Ihren Zielen entspricht.

## Welchen Sinn hat es, sie jetzt zu kaufen, wenn das OHM mit einem sehr hohen Aufschlag gehandelt wird?

Wenn Sie OHM kaufen und einsetzen, erwerben Sie einen prozentualen Anteil des Angebots \(Marktkapitalisierung\), der nahezu konstant bleibt. Dies liegt daran, dass Ihr OHM-Einsatz mit dem zirkulierenden Angebot steigt. Wenn Sie also OHM kaufen, wenn die Marktkapitalisierung niedrig ist, erhalten Sie einen größeren Anteil an der Marktkapitalisierung.

## Was ist eine Rebase?

Rebase ist ein Mechanismus, durch den sich Ihr eingesetztes OHM-Guthaben automatisch erhöht. Wenn neue OHM durch das Protokoll geprägt werden, geht ein großer Teil davon an die Staker. Da die Staker nur das eingesetzte OHM-Guthaben und nicht die OHM sehen, nutzt das Protokoll den Rebase-Mechanismus, um das eingesetzte OHM-Guthaben zu erhöhen, so dass 1 eingesetztes OHM immer für 1 OHM eingelöst werden kann.

## Was ist die Reward Yield?

Der Reward Yield ist der Prozentsatz, um den sich Ihr eingesetztes OHM-Guthaben in der nächsten Epoche erhöht. Sie wird auch als Rebase-Rate bezeichnet. Sie finden diese Zahl auf der [Olympus Staking-Seite](https://app.olympusdao.finance/#/stake).

## Was ist APY?

APY steht für annualisierte prozentuale Rendite. Er misst die reale Rendite Ihres Kapitals, indem er den Effekt des Zinseszinses berücksichtigt. Im Fall von OlympusDAO stellt Ihr eingesetztes OHM Ihr Kapital dar, und der Zinseszins wird dank des Rebase-Mechanismus periodisch in jeder Epoche \(2200 Ethereum-Blöcke oder etwa 8 Stunden\) hinzugefügt.

Eine interessante Tatsache über APY ist, dass Ihr Guthaben nicht linear, sondern exponentiell mit der Zeit wächst! Geht man von einem täglichen Zinseszins von 2 % aus, so wird Ihr Guthaben, wenn Sie am ersten Tag mit einem Guthaben von 1 OHM beginnen, nach einem Jahr auf etwa 1377 OHM anwachsen. Das ist eine ganze Menge!

![Die Macht der Zinseszinsen](../.gitbook/assets/apy.png)

## Wie wird die APY berechnet?

Der APY errechnet sich aus der Rendite \(auch bekannt als Rebase Rate\) anhand der folgenden Gleichung:

$$
APY = ( 1 + rewardYield )^{1095}
$$

Sie erhöht sich hoch 1095, weil ein Rebase 3 Mal täglich stattfindet. Da ein Jahr 365 Tage hat, ergibt sich eine Rebase-Häufigkeit von 365 \* 3 = 1095.

Der Ertrag der Belohnung wird durch die folgende Gleichung bestimmt:

$$
rewardYield = OHM_{distributed} / OHM_{totalStaked}
$$

Die Anzahl der auf den Staking-contract verteilten OHM wird anhand der folgenden Gleichung aus dem Gesamtangebot an OHM berechnet:

$$
OHM_{distributed} = OHM_{totalSupply} \times rewardRate
$$

Beachten Sie, dass der Belohnungssatz durch das Protokoll geändert werden kann. So wurde er beispielsweise aufgrund dieses [jüngsten Vorschlags](https://forum.olympusdao.finance/d/77-oip-18-reward-rate-framework-and-reduction) überarbeitet.

## Warum wird der Preis des OHM langfristig irrelevant?

Wie oben dargestellt, wächst Ihr OHM-Guthaben im Laufe der Zeit dank der Macht der Zinseszinsen exponentiell. Nehmen wir an, Sie kaufen jetzt ein OHM für 400 $ und der Markt entscheidet, dass der innere Wert des OHM in einem Jahr bei 2 $ liegen wird. Bei einem täglichen Zinseszins von 2 % würde Ihr Guthaben bis zum Ende des Jahres auf etwa 1377 OHMs anwachsen, die etwa 2754 $ wert sind. Das ist ein toller Gewinn von $2354! Inzwischen sollten Sie verstanden haben, dass Sie jetzt eine Prämie für OHM zahlen und dafür einen langfristigen Nutzen erhalten. Sie sollten also einen langen Zeithorizont haben, damit Ihr OHM-Guthaben exponentiell wachsen kann und sich diese Investition lohnt.

## Wie hoch wird der intristische Wert von OHM in Zukunft sein?

Hierauf gibt es keine eindeutige Antwort, aber der intristische Wert kann durch die Leistung des Schatzamtes bestimmt werden. Wenn das Schatzamt zum Beispiel garantieren könnte, jedes OHM mit 100 DAI zu unterlegen, wäre der innere Wert 100 DAI. Er kann auch von der DAO bestimmt werden. Wenn die [DAO zum Beispiel](https://forum.olympusdao.finance/d/31-use-price-floor-as-tool-for-monetary-policy) beschließt, die Preisuntergrenze für OHM anzuheben, wird der innere Wert entsprechend steigen.

## Wie schafft es das Protokoll, den hohen Staking-APY zu halten?

Nehmen wir an, das Protokoll strebt einen effektiven Jahreszins von 100.000% an. Dies entspräche einem Basiszinssatz von etwa 0,6328 % oder einem täglichen Wachstum von etwa 2 %. In der obigen Gleichung erfahren Sie, wie der [APY aus der Rebase-Rate](basics.md#wie-wird-die-apy-berechnet) berechnet wird.

Wenn jetzt 100.000 OHM staked sind, müsste das Protokoll zusätzlich 2000 OHM prägen, um dieses tägliche Wachstum zu erreichen. Dies ist möglich, wenn das Protokoll täglich mindestens 2000 DAI aus Bondverkäufen einbringen kann. Wenn das Protokoll dies nicht erreicht, kann der APY von 100.000% nicht garantiert werden.

## Muss ich in jeder Epoche meine OHM unstaken und neu staken, um meine Rebase-Belohnungen zu erhalten?

Nein. Sobald Sie OHM bei OlympusDAO gestaked haben, erhöht sich Ihr gestakedes OHM-Guthaben in jeder Epoche automatisch. Dieser Anstieg des Guthabens entspricht Ihrer Rebase-Belohnung.

## Wie kann ich meine Rebase-Belohnungen verfolgen?

Sie können Ihre Rebase-Belohnungen nachverfolgen, indem Sie den Anstieg Ihres OHM-Einsatzes berechnen.

1. Notieren Sie den aktuellen Indexwert auf der [Staking-Seite](https://app.olympusdao.finance/#/stake), wenn Sie Ihren OHM zum ersten Mal einsetzen. Nennen wir dies den Startindex.

![](../.gitbook/assets/index_old.png)

2. Wenn Sie nach einiger Zeit feststellen möchten, um wie viel sich Ihr Guthaben erhöht hat, überprüfen Sie erneut den aktuellen Indexwert. Wir nennen dies den Endindex.

![](../.gitbook/assets/index_new.png)

3. Wenn Sie den Endindex durch den Startindex dividieren, erhalten Sie das Verhältnis, um das sich Ihr eingesetzter OHM-Saldo erhöht hat.

$$
ratio = endIndex / startIndex
$$

4. In diesem Beispiel ist der OHM-Saldo um das 1,5-fache gestiegen.

$$
ratio = 13.2\ /\ 8.8\newline = 1.5
$$

