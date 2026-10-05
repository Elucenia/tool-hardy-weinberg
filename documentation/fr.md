<!-- ELUCENIA technical documentation · hardy-weinberg · fr · no clinical/professional/rights approval -->

# Équilibre de Hardy-Weinberg

[conditions, sources et autorisations](https://elucenia.org/fr/outils/hardy-weinberg)

## Mode d’emploi

Utilisez l’outil sur le portail ou ouvrez index.html via un serveur HTTP local. Sélectionnez la langue, remplissez les champs et lancez le calcul.

## Données d’entrée et unités

### Fréquence de la maladie : 1 personne atteinte sur

`incid`

naissances · intervalle: 100–1000000

### Partenaire 1

`p1`

- `pop` — Population générale
- `port` — Porteur confirmé
- `irmao` — Frère ou sœur non atteint d’une personne atteinte

### Partenaire 2

`p2`

- `pop` — Population générale
- `port` — Porteur confirmé
- `irmao` — Frère ou sœur non atteint d’une personne atteinte

## Édition de la méthode

Hardy–Weinberg 1908 : p²+2pq+q² ; transmission autosomique récessive ; frère/sœur non atteint 2/3 ; risque du couple ×1/4

## Formule documentée

À l’équilibre : p² + 2pq + q² = 1, q étant la fréquence de l’allèle pathogène et p = 1 − q.

Incidence = q², donc q = √incidence.

Fréquence des porteurs (hétérozygotes) = 2pq (≈ 2q si q est petit).

Probabilité que chaque partenaire soit porteur : population générale = 2pq ; porteur confirmé = 1 ; frère ou sœur non atteint d’une personne atteinte = 2/3.

Risque par grossesse = P(partenaire 1 porteur) × P(partenaire 2 porteur) × 1/4.

## Limites et population

Le calcul populationnel suppose un locus autosomique à deux allèles en équilibre de Hardy–Weinberg ; l’accouplement aléatoire et une population idéalement très grande sont des hypothèses, pas des résultats du calcul. Utiliser q² comme fréquence de la maladie exige une concordance avec le modèle récessif considéré. Le risque familial de 25% suppose deux parents porteurs ; les 2/3 pour un membre de la fratrie non atteint constituent une probabilité conditionnelle dans ce scénario. N’appliquez pas ces relations à toute maladie génétique et ne les interprétez pas comme un diagnostic individuel.

## Références

- [Hardy GH. Mendelian proportions in a mixed population. Science, 1908.](https://doi.org/10.1126/science.28.706.49)

- [Mayo O. A century of Hardy-Weinberg equilibrium. Twin Res Hum Genet, 2008.](https://doi.org/10.1375/twin.11.3.249)

- [GeneReviews carrier box,revised2016](https://www.ncbi.nlm.nih.gov/books/NBK5191/box/further_illus-19/)

## Reproduire les tests techniques

Exécutez node test.cjs dans le répertoire racine de ce dépôt pour reproduire les cas synthétiques enregistrés. Les données d’entrée, les résultats attendus et les tolérances d’origine sont conservés. Les tests techniques ne constituent pas une validation clinique.

```sh
node test.cjs
```

tool.json contient les sources, l’édition et le périmètre de la revue. examples.json conserve les données d’entrée et les résultats attendus des cas synthétiques ; results.json consigne les résultats obtenus.

[Fiche et références](../tool.json) · [Code JavaScript](../calculator.js) · [Cas de référence](../examples.json) · [results.json](../results.json)

## Revue et conditions d’utilisation

Aucune révision clinique indépendante n’a été effectuée.

Cette interface est une traduction réalisée par nos soins, et non une édition officielle ou certifiée. La revue clinique indépendante, la révision linguistique professionnelle et l’autorisation des droits sur les instruments n’ont pas été réalisées.

Résultat de la formule ou de la classification. L’interprétation, la conduite et l’applicabilité dépendent de l’évaluation professionnelle et de la source sélectionnée.

## Licence et attribution

Apache-2.0 s’applique uniquement au code d’ELUCENIA. Les droits sur les instruments, publications, traductions et données restent ceux de leurs titulaires respectifs. Conservez LICENSE et NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026
