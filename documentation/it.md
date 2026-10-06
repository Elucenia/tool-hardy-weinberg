<!-- ELUCENIA technical documentation · hardy-weinberg · it · no clinical/professional/rights approval -->

# Equilibrio di Hardy-Weinberg

[condizioni, fonti e autorizzazioni](https://elucenia.org/it/strumenti/hardy-weinberg)

## Come usare

Usi lo strumento nel portale oppure apra index.html tramite un server HTTP locale. Selezioni la lingua, compili i campi ed esegua il calcolo.

## Dati di ingresso e unità

### Frequenza della malattia: 1 persona affetta ogni

`incid`

nati · intervallo: 100–1000000

### Partner 1

`p1`

- `pop` — Popolazione generale
- `port` — Portatore confermato
- `irmao` — Fratello o sorella non affetto di una persona affetta

### Partner 2

`p2`

- `pop` — Popolazione generale
- `port` — Portatore confermato
- `irmao` — Fratello o sorella non affetto di una persona affetta

## Edizione del metodo

Hardy–Weinberg 1908: p²+2pq+q²; ereditarietà autosomica recessiva; fratello non affetto 2/3; rischio di coppia ×1/4

## Formula documentata

In equilibrio: p² + 2pq + q² = 1; q è la frequenza dell’allele patogeno e p = 1 − q.

Incidenza = q², quindi q = √incidenza.

Frequenza dei portatori (eterozigoti) = 2pq (≈ 2q se q è piccolo).

Probabilità di essere portatore per ogni partner: popolazione generale = 2pq; portatore confermato = 1; fratello non affetto di una persona affetta = 2/3.

Rischio per gravidanza = P(partner 1 portatore) × P(partner 2 portatore) × 1/4.

## Limiti e popolazione

Il calcolo di popolazione presuppone un locus autosomico con due alleli in equilibrio di Hardy–Weinberg; accoppiamento casuale e popolazione idealmente molto grande sono ipotesi, non risultati del calcolo. Usare q² come frequenza della malattia richiede corrispondenza con il modello recessivo considerato. Il rischio familiare del 25% presuppone due genitori portatori; i 2/3 per un fratello o una sorella non affetti sono una probabilità condizionata in quello scenario. Non applicare queste relazioni a qualsiasi malattia genetica né interpretarle come diagnosi individuale.

## Riferimenti

- [Hardy GH. Mendelian proportions in a mixed population. Science, 1908.](https://doi.org/10.1126/science.28.706.49)

- [Mayo O. A century of Hardy-Weinberg equilibrium. Twin Res Hum Genet, 2008.](https://doi.org/10.1375/twin.11.3.249)

- [GeneReviews carrier box,revised2016](https://www.ncbi.nlm.nih.gov/books/NBK5191/box/further_illus-19/)

## Riprodurre i test tecnici

Esegua node test.cjs nella cartella principale di questo repository per ripetere i casi sintetici registrati. Gli input, i risultati attesi e le tolleranze originali sono conservati. I test tecnici non costituiscono validazione clinica.

```sh
node test.cjs
```

tool.json contiene le fonti, l’edizione e l’ambito della revisione. examples.json conserva gli input e i risultati attesi dei casi sintetici; results.json registra i risultati ottenuti.

[Scheda e riferimenti](../tool.json) · [Codice JavaScript](../calculator.js) · [Casi di riferimento](../examples.json) · [results.json](../results.json)

## Revisione e condizioni d’uso

Non è stata effettuata una revisione clinica indipendente.

Questa interfaccia è una traduzione realizzata dagli autori, non un’edizione ufficiale o certificata. Non sono state eseguite la revisione clinica indipendente, la revisione linguistica professionale né la verifica delle autorizzazioni relative ai diritti sugli strumenti.

Risultato della formula o classificazione. Interpretazione, condotta e applicabilità dipendono dalla valutazione professionale e dalla fonte selezionata.

## Licenza e attribuzione

Apache-2.0 si applica solo al codice di ELUCENIA. I diritti su strumenti, pubblicazioni, traduzioni e dati restano ai rispettivi titolari. Conservi LICENSE e NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026

## Risultati documentati

Le informazioni seguenti conservano gli output del metodo per esempi sintetici. Non costituiscono una validazione clinica indipendente.

### 1

Frequenza dei portatori nella popolazione: 1 su 26

| Dettagli del risultato | |
| --- | --- |
| Frequenza allelica (q) | 2,00% |
| Frequenza dei portatori (2pq) | 3,92% (1 su 26) |
| Rischio della coppia per gravidanza | 0,038% |


### 2

Frequenza dei portatori nella popolazione: 1 su 26

| Dettagli del risultato | |
| --- | --- |
| Frequenza allelica (q) | 2,00% |
| Frequenza dei portatori (2pq) | 3,92% (1 su 26) |
| Rischio della coppia per gravidanza | 0,980% |


### 3

Frequenza dei portatori nella popolazione: 1 su 26

| Dettagli del risultato | |
| --- | --- |
| Frequenza allelica (q) | 2,00% |
| Frequenza dei portatori (2pq) | 3,92% (1 su 26) |
| Rischio della coppia per gravidanza | 0,653% |


### 4

Frequenza dei portatori nella popolazione: 1 su 51

| Dettagli del risultato | |
| --- | --- |
| Frequenza allelica (q) | 1,00% |
| Frequenza dei portatori (2pq) | 1,98% (1 su 51) |
| Rischio della coppia per gravidanza | 25,000% |


### 5

Frequenza dei portatori nella popolazione: 1 su 51

| Dettagli del risultato | |
| --- | --- |
| Frequenza allelica (q) | 1,00% |
| Frequenza dei portatori (2pq) | 1,98% (1 su 51) |
| Rischio della coppia per gravidanza | 0,010% |

