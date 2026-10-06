<!-- ELUCENIA technical documentation · hardy-weinberg · en · no clinical/professional/rights approval -->

# Hardy–Weinberg equilibrium

[conditions, sources and permissions](https://elucenia.org/en/tools/hardy-weinberg)

## How to use

Use the tool in the portal or open index.html through a local HTTP server. Select the language, complete the fields and calculate.

## Inputs and units

### Disease frequency: 1 affected person per

`incid`

births · range: 100–1000000

### Partner 1

`p1`

- `pop` — General population
- `port` — Confirmed carrier
- `irmao` — Unaffected sibling of an affected person

### Partner 2

`p2`

- `pop` — General population
- `port` — Confirmed carrier
- `irmao` — Unaffected sibling of an affected person

## Method edition

Hardy–Weinberg 1908: p²+2pq+q²; autosomal recessive inheritance; unaffected sibling 2/3; couple risk ×1/4

## Documented formula

At equilibrium: p² + 2pq + q² = 1, where q is the pathogenic allele frequency and p = 1 − q.

Disease incidence = q², so q = √incidence.

Carrier frequency (heterozygotes) = 2pq (≈ 2q when q is small).

Each partner’s carrier probability: general population = 2pq; confirmed carrier = 1; unaffected sibling of an affected individual = 2/3.

Risk per pregnancy = P(partner 1 carrier) × P(partner 2 carrier) × 1/4.

## Limits and population

The population calculation assumes an autosomal locus with two alleles in Hardy–Weinberg equilibrium; random mating and an ideally very large population are assumptions, not outputs of the calculation. Using q² as disease frequency requires agreement with the recessive model considered. A familial risk of 25% assumes two carrier parents; the 2/3 for an unaffected sibling is a conditional probability in that setting. Do not apply these relationships to every genetic disease or interpret them as an individual diagnosis.

## References

- [Hardy GH. Mendelian proportions in a mixed population. Science, 1908.](https://doi.org/10.1126/science.28.706.49)

- [Mayo O. A century of Hardy-Weinberg equilibrium. Twin Res Hum Genet, 2008.](https://doi.org/10.1375/twin.11.3.249)

- [GeneReviews carrier box,revised2016](https://www.ncbi.nlm.nih.gov/books/NBK5191/box/further_illus-19/)

## Reproduce the technical tests

Run node test.cjs in the root directory of this repository to repeat the recorded synthetic cases. Original inputs, expectations and tolerances are preserved. Technical tests do not constitute clinical validation.

```sh
node test.cjs
```

tool.json contains sources, edition and review scope. examples.json retains synthetic inputs and expectations; results.json records the obtained results.

[Record and references](../tool.json) · [JavaScript code](../calculator.js) · [Reference cases](../examples.json) · [results.json](../results.json)

## Review and conditions of use

Independent clinical review has not been performed.

This interface is an authorial translation, not an official or certified edition. Independent clinical review, professional language review and instrument rights clearance have not been performed.

Formula or classification result. Interpretation, care and applicability depend on professional assessment and the selected source.

## License and attribution

Apache-2.0 applies only to ELUCENIA code. Rights to instruments, publications, translations and data remain with their respective holders. Preserve LICENSE and NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026

## Documented results

The information below preserves the method outputs for synthetic examples. It does not constitute independent clinical validation.

### 1

Carrier frequency in the population: 1 in 26

| Result details | |
| --- | --- |
| Allele frequency (q) | 2.00% |
| Carrier frequency (2pq) | 3.92% (1 in 26) |
| Couple risk per pregnancy | 0.038% |


### 2

Carrier frequency in the population: 1 in 26

| Result details | |
| --- | --- |
| Allele frequency (q) | 2.00% |
| Carrier frequency (2pq) | 3.92% (1 in 26) |
| Couple risk per pregnancy | 0.980% |


### 3

Carrier frequency in the population: 1 in 26

| Result details | |
| --- | --- |
| Allele frequency (q) | 2.00% |
| Carrier frequency (2pq) | 3.92% (1 in 26) |
| Couple risk per pregnancy | 0.653% |


### 4

Carrier frequency in the population: 1 in 51

| Result details | |
| --- | --- |
| Allele frequency (q) | 1.00% |
| Carrier frequency (2pq) | 1.98% (1 in 51) |
| Couple risk per pregnancy | 25.000% |


### 5

Carrier frequency in the population: 1 in 51

| Result details | |
| --- | --- |
| Allele frequency (q) | 1.00% |
| Carrier frequency (2pq) | 1.98% (1 in 51) |
| Couple risk per pregnancy | 0.010% |

