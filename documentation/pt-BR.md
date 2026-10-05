<!-- ELUCENIA technical documentation · hardy-weinberg · pt-BR · no clinical/professional/rights approval -->

# Equilíbrio de Hardy-Weinberg

[condições, fontes e permissões](https://elucenia.org/pt-br/ferramentas/hardy-weinberg)

## Como usar

Use a ferramenta no portal ou abra index.html em um servidor HTTP local. Selecione o idioma, preencha os campos e calcule.

## Entradas e unidades

### Incidência da doença: 1 afetado a cada

`incid`

nascidos · intervalo: 100–1000000

### Parceiro 1

`p1`

- `pop` — População geral
- `port` — Portador confirmado
- `irmao` — Irmão(ã) não afetado de um afetado

### Parceiro 2

`p2`

- `pop` — População geral
- `port` — Portador confirmado
- `irmao` — Irmão(ã) não afetado de um afetado

## Edição do método

Hardy Weinberg 1908:p²+2 pq+q²; herança AR; irmão nãoafetado 2/3; risco conjugal×1/4

## Fórmula documentada

Em equilíbrio: p² + 2pq + q² = 1, em que q é a frequência do alelo patogênico e p = 1 − q.

Incidência da doença = q², logo q = √incidência.

Frequência de portadores (heterozigotos) = 2pq (≈ 2q quando q é pequeno).

Probabilidade de cada parceiro ser portador: população geral = 2pq; portador confirmado = 1; irmão não afetado de um afetado = 2/3.

Risco por gestação = P(parceiro 1 portador) × P(parceiro 2 portador) × 1/4.

## Limites e população

O cálculo populacional assume um locus autossômico com dois alelos em equilíbrio de Hardy–Weinberg; acasalamento aleatório e uma população idealmente muito grande são pressupostos, não resultados do cálculo. Usar q² como frequência da doença exige correspondência com o modelo recessivo considerado. O risco familiar de 25% pressupõe dois pais portadores; os 2/3 para um irmão não afetado são uma probabilidade condicional nesse cenário. Não aplique essas relações a qualquer doença genética nem as interprete como diagnóstico individual.

## Referências

- [Hardy GH. Mendelian proportions in a mixed population. Science, 1908.](https://doi.org/10.1126/science.28.706.49)

- [Mayo O. A century of Hardy-Weinberg equilibrium. Twin Res Hum Genet, 2008.](https://doi.org/10.1375/twin.11.3.249)

- [GeneReviews carrier box,revised2016](https://www.ncbi.nlm.nih.gov/books/NBK5191/box/further_illus-19/)

## Reproduzir os testes técnicos

Execute node test.cjs na pasta raiz deste repositório para repetir os casos sintéticos registrados. As entradas, expectativas e tolerâncias originais são preservadas. Testes técnicos não constituem validação clínica.

```sh
node test.cjs
```

tool.json contém fontes, edição e escopo de revisão. examples.json conserva as entradas e expectativas sintéticas; results.json registra os resultados obtidos.

[Ficha e referências](../tool.json) · [Código JavaScript](../calculator.js) · [Casos de referência](../examples.json) · [results.json](../results.json)

## Revisão e condições de uso

Revisão clínica independente não realizada.

Esta interface é uma tradução autoral, não uma edição oficial ou certificada. Revisão clínica independente, revisão linguística profissional e autorização de direitos de instrumentos não foram realizadas.

Resultado da fórmula ou classificação. Interpretação, conduta e aplicabilidade dependem da avaliação profissional e da fonte selecionada.

## Licença e atribuição

Apache-2.0 aplica-se somente ao código da ELUCENIA. Os instrumentos, publicações, traduções e dados mantêm os direitos dos respectivos titulares. Preserve LICENSE e NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026
