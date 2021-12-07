---
description: Zur Umstellung auf Version 2 (V2)
---

# V2-Migration

## Warum muss ich auf Version 2 umstellen?

Die Umstellung auf V2 führt neue Funktionen ein, darunter erweiterte Mitbestimmung (on-chain governance) und automatisches Staken für Anleihen.

Der Übergang von sOHM V1 auf gOHM ermöglicht mehrere Anleihen gleichzeitig, anstelle von einer Anleihe je Anlagezeitraum, wie es bisher in V1 der Fall war.

So lange die Umstellung im Gange ist, wird ein Teil der Liquidität weiterhin für v1 OHM bereitgestellt. Das soll sicherstellen, dass genug Liquidität für Kreditnehmer vorhanden ist, um die Darlehen zu begleichen oder zu transferieren.

Mehr dazu steht auf dieser [Olympus Medium-Seite](https://olympusdao.medium.com/introducing-olympus-v2-c4ade14e9fe).

{% hint style="info" %}
**Nach dem Start von V2 bleiben zwei Monate Zeit, um die Token zu migrieren.** Danach wird das Guthaben an sOHM nicht mehr weiter verzinst, aber die Differenz wird angerechnet, sobald später eine Migration erfolgt.
{% endhint %}

{% hint style="info" %}
In diesem Artikel steht V1 und V2 hinter jeder Token-Bezeichnung, um die Unterscheidung zwischen alten und neuen Token zu erleichtern. Partner-Seiten, Preis-Portale und Wallets werden die Version nicht anzeigen.
{% endhint %}

## Was heißt das, knapp zusammengefasst (TL;DR)?

* wsOHM V1 (gewrapptes gestaktes OHM) wird durch gOHM (Governance OHM) ersetzt. Beide funktionieren genau gleich, aber gOHM ist auf die erweiterte Mitbestimmung (on-chain governance) ausgelegt.
* OHM- und sOHM-Token haben identische V2-Versionen: OHM V1 wird zu OHM V2, und sOHM V1 wird zu sOHM V2.
* Die Token-Anzeige wird für V1-Token gleich bleiben. Nach der Migration wird die Wallet beispielsweise "OHM" statt "OHM V1" anzeigen. Der Token-Kontrakt in der Wallet muss mit den [V2-Adressen](https://app.gitbook.com/s/-MV4hwONledQK5nEDaUc-887967055/contracts/tokens) aktualisiert werden, damit das Guthaben angezeigt werden kann.
* Beim Migrieren von OHM V1 und/oder sOHM V1 erhält man im Austausch gOHM. Dieses Token-Guthaben wird sich unterscheiden (der Preis für gOHM wird anders berechnet, da er auf dem Current Index basiert), aber **der Wert in US-Dollar ist identisch**.
* Nach der Umstellung werden OHM V1-Pools wie etwa OHM-DAI künftig OHM V2 nutzen. Das gilt auch für neue Anleihen. Partner wie Abracadabra werden neue Investitionen nur noch in gOHM akzeptieren. Um diese Möglichkeiten zu nutzen, ist es also unerlässlich, zu migrieren. Wer daran nicht interessiert ist, kann vorerst auch einfach nichts tun und erst später nach Belieben umstellen.

## Und wenn ich nicht migriere?

Dann kann man leider die neuen Features nicht nutzen, die V2 einführt. Einige Partner wie etwa Rari Capital werden nur V2-Token akzeptieren, sobald sie freigeschaltet sind. Um dort zu investieren (also um z.B. neu einzuzahlen), ist es unerlässlich, auf V2 zu migrieren.

## Die Gas-Gebühren sind gerade so hoch. Verliere ich meine Rebase-Zinsen, wenn ich die Umstellung später durchführe?

Nein, man kann jederzeit umstellen, sobald Version 2 live ist. Der Smart Contract wird sich den Anspruch auf die Zinsen merken, so dass man keine davon verliert.

## Wie geht die Umstellung vor sich?

Sobald die Umstellung live ist, werden wir die Olympus DApp-Seite aktualisieren, um die Umstellung aller V1-OHM-Token (also OHM, sOHM und wsOHM) auf gOHM zu ermöglichen.

Die Umstellung selbst erfordert zwei Schritte: einen, um den Vorgang für jeden der V1-Token zu autorisieren, und einen zweiten, um die eigentliche Umstellung vorzunehmen und alle Token in gOHM umzuwandeln.

{% hint style="info" %}
Jeder V1-Token erfordert seinen eigenen Autorisierungs-Schritt. Wer beispielsweise OHM V1 und sOHM V1 in seiner Wallet hält, muss zwei Autorisierungsschritte durchführen, aber nur einen Umwandlungs-Schritt (insgesamt 3 Transaktionen).
{% endhint %}

## Kann ich eine Art von Token umstellen und die anderen aussparen?

Nein. Man kann nur entweder alle V1-Token (sprich OHM, sOHM und wsOHM) umstellen oder gar keinen.

## Kann ich gOHM wieder zurück in V1-Token umwandeln?

Nein, mit unserem Migrations-Tool kann man gOHM nicht zurück in V1-Token umwandeln.

## Könnte ich mal an einem Beispiel sehen, wie viel gOHM ich nach der Umstellung erhalten würde?

Nehmen wir an, jemand hat 20 OHM V1, 20 sOHM V1 und 20 wsOHM. Der [Current Index](https://docs.olympusdao.finance/main/basics/basics#how-do-i-track-my-rebase-rewards) beträgt 10.

* 20 OHM V1 = 2 gOHM (Man nehme die 20 OHM und teile sie durch den Current Index um gOHM zu erhalten.)
* 20 sOHM V1 = 2 gOHM (Man nehme die 20 sOHM und teile sie durch den Current Index um gOHM zu erhalten.)
* 20 wsOHM = 20 gOHM (1 wsOHM entspricht 1 gOHM.)

{% hint style="info" %}
Zur Erinnerung: Wer von einem nicht-index-basierten Token (OHM, sOHM) auf einen index-basierten Token migriert, erhält nach der Umstellung nicht dieselbe Menge an Token, aber der Wert ausgedrückt in US-Dollar bleibt dennoch unverändert.
{% endhint %}

## Wird mein gOHM weiterhin verzinst?

Ja. Auch wenn sich gOHM nicht so wie sOHM nach jeder Ausschüttungsrunde vermehrt, erwirtschaftet es dennoch Zinserträge. Das liegt daran, dass gOHM an den Current Index gebunden ist:

$$
gOHMprice = OHMprice * CurrentIndex
$$

Jede Ausschüttungsrunde erhöht den Current Index, folglich ist gOHM danach mehr wert (vorausgesetzt, der Preis für OHM bleibt konstant).

## Welche Auswirkungen hat die Migration auf Anleihen?

In V2 kann man mehrere Anleihen der gleichen Art erwerben, ohne dass der Anlagezeitraum jeweils neu von vorne beginnt.

Es ist auch nicht nötig, die Anleihe-Zinsen einzufordern und neu zu staken, das passiert jetzt automatisch. Bonder erhalten die ihnen zustehenden sOHM am Ende des Anlagezeitraums.

Mehr dazu, wie sich Anleihen in V2 verhalten, steht auf dieser [Olympus Medium-Seite](https://olympusdao.medium.com/introducing-olympus-v2-c4ade14e9fe).

## Gibt es für Olympus V2 eine externe Sicherheitsprüfung?

Alle V2-Kontrakte sind live, einige davon unterliegen einer noch laufenden Prüfung. Für die Scherheitsprüfung arbeiten wir mit Runtime Verification zusammen, und die Ergebnisse werden veröffentlicht, sobald sie verfügbar sind.

\
\
