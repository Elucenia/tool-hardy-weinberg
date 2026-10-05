<!-- ELUCENIA technical documentation · hardy-weinberg · de · no clinical/professional/rights approval -->

# Hardy-Weinberg-Gleichgewicht

[Bedingungen, Quellen und Berechtigungen](https://elucenia.org/de/werkzeuge/hardy-weinberg)

## Verwendung

Verwenden Sie das Werkzeug im Portal oder öffnen Sie index.html über einen lokalen HTTP-Server. Wählen Sie die Sprache, füllen Sie die Felder aus und berechnen Sie das Ergebnis.

## Eingaben und Einheiten

### Krankheitshäufigkeit: 1 betroffene Person pro

`incid`

Geburten · Bereich: 100–1000000

### Partner 1

`p1`

- `pop` — Allgemeinbevölkerung
- `port` — Bestätigter Anlageträger
- `irmao` — Nicht betroffene Geschwisterperson einer betroffenen Person

### Partner 2

`p2`

- `pop` — Allgemeinbevölkerung
- `port` — Bestätigter Anlageträger
- `irmao` — Nicht betroffene Geschwisterperson einer betroffenen Person

## Fassung der Methode

Hardy–Weinberg 1908: p²+2pq+q²; autosomal-rezessiver Erbgang; nicht betroffenes Geschwister 2/3; Paar-Risiko ×1/4

## Dokumentierte Formel

Im Gleichgewicht: p² + 2pq + q² = 1; q ist die Häufigkeit des pathogenen Allels, p = 1 − q.

Erkrankungsinzidenz = q², somit q = √Inzidenz.

Trägerhäufigkeit (Heterozygote) = 2pq (≈ 2q bei kleinem q).

Trägerwahrscheinlichkeit je Partner: Allgemeinbevölkerung = 2pq; bestätigter Träger = 1; nicht betroffenes Geschwister einer betroffenen Person = 2/3.

Risiko je Schwangerschaft = P(Partner 1 Träger) × P(Partner 2 Träger) × 1/4.

## Grenzen und Population

Die Populationsberechnung setzt einen autosomalen Locus mit zwei Allelen im Hardy–Weinberg-Gleichgewicht voraus. Zufällige Paarung und eine idealerweise sehr große Population sind Annahmen, keine Rechenergebnisse. q² als Krankheitshäufigkeit zu verwenden erfordert Übereinstimmung mit dem betrachteten rezessiven Modell. Ein familiäres Risiko von 25% setzt zwei Anlageträger als Eltern voraus; die 2/3 für ein nicht betroffenes Geschwister sind in diesem Szenario eine bedingte Wahrscheinlichkeit. Wenden Sie diese Beziehungen nicht auf jede genetische Erkrankung an und interpretieren Sie sie nicht als individuelle Diagnose.

## Referenzen

- [Hardy GH. Mendelian proportions in a mixed population. Science, 1908.](https://doi.org/10.1126/science.28.706.49)

- [Mayo O. A century of Hardy-Weinberg equilibrium. Twin Res Hum Genet, 2008.](https://doi.org/10.1375/twin.11.3.249)

- [GeneReviews carrier box,revised2016](https://www.ncbi.nlm.nih.gov/books/NBK5191/box/further_illus-19/)

## Technische Tests reproduzieren

Führen Sie node test.cjs im Stammverzeichnis dieses Repositorys aus, um die dokumentierten synthetischen Fälle zu wiederholen. Ursprüngliche Eingaben, erwartete Ergebnisse und Toleranzen bleiben erhalten. Technische Tests stellen keine klinische Validierung dar.

```sh
node test.cjs
```

tool.json enthält Quellen, Ausgabe und Umfang der Überprüfung. examples.json bewahrt die synthetischen Eingaben und erwarteten Ergebnisse; results.json dokumentiert die tatsächlich erhaltenen Ergebnisse.

[Eintrag und Referenzen](../tool.json) · [JavaScript-Code](../calculator.js) · [Referenzfälle](../examples.json) · [results.json](../results.json)

## Überprüfung und Nutzungsbedingungen

Eine unabhängige klinische Prüfung wurde nicht durchgeführt.

Diese Benutzeroberfläche ist eine selbst erstellte Übersetzung und keine offizielle oder zertifizierte Ausgabe. Eine unabhängige klinische Überprüfung, eine professionelle sprachliche Prüfung und eine Klärung der Rechte an den Instrumenten wurden nicht durchgeführt.

Ergebnis der Formel oder Klassifikation. Interpretation, Vorgehen und Anwendbarkeit hängen von der fachlichen Beurteilung und der ausgewählten Quelle ab.

## Lizenz und Urheberangaben

Apache-2.0 gilt nur für den ELUCENIA-Code. Die Rechte an Instrumenten, Veröffentlichungen, Übersetzungen und Daten verbleiben bei den jeweiligen Rechteinhabern. Bewahren Sie LICENSE und NOTICE auf.

ELUCENIA · Felipe Guedes · Copyright © 2026
