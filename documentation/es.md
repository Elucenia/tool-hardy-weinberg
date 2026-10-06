<!-- ELUCENIA technical documentation · hardy-weinberg · es · no clinical/professional/rights approval -->

# Equilibrio de Hardy-Weinberg

[condiciones, fuentes y permisos](https://elucenia.org/es/herramientas/hardy-weinberg)

## Cómo usar

Utilice la herramienta en el portal o abra index.html mediante un servidor HTTP local. Seleccione el idioma, complete los campos y calcule.

## Entradas y unidades

### Frecuencia de la enfermedad: 1 afectado por cada

`incid`

nacimientos · intervalo: 100–1000000

### Pareja 1

`p1`

- `pop` — Población general
- `port` — Portador confirmado
- `irmao` — Hermano no afectado de una persona afectada

### Pareja 2

`p2`

- `pop` — Población general
- `port` — Portador confirmado
- `irmao` — Hermano no afectado de una persona afectada

## Edición del método

Hardy–Weinberg 1908: p²+2pq+q²; herencia autosómica recesiva; hermano no afectado 2/3; riesgo de pareja ×1/4

## Fórmula documentada

En equilibrio: p² + 2pq + q² = 1, donde q es la frecuencia del alelo patógeno y p = 1 − q.

Incidencia = q², por tanto q = √incidencia.

Frecuencia de portadores (heterocigotos) = 2pq (≈ 2q si q es pequeño).

Probabilidad de que cada integrante sea portador: población general = 2pq; portador confirmado = 1; hermano no afectado de una persona afectada = 2/3.

Riesgo por embarazo = P(integrante 1 portador) × P(integrante 2 portador) × 1/4.

## Límites y población

El cálculo poblacional presupone un locus autosómico con dos alelos en equilibrio de Hardy–Weinberg; el apareamiento aleatorio y una población idealmente muy grande son supuestos, no resultados del cálculo. Usar q² como frecuencia de la enfermedad exige correspondencia con el modelo recesivo considerado. El riesgo familiar del 25% presupone dos progenitores portadores; los 2/3 para un hermano no afectado son una probabilidad condicional en ese escenario. No aplique estas relaciones a cualquier enfermedad genética ni las interprete como diagnóstico individual.

## Referencias

- [Hardy GH. Mendelian proportions in a mixed population. Science, 1908.](https://doi.org/10.1126/science.28.706.49)

- [Mayo O. A century of Hardy-Weinberg equilibrium. Twin Res Hum Genet, 2008.](https://doi.org/10.1375/twin.11.3.249)

- [GeneReviews carrier box,revised2016](https://www.ncbi.nlm.nih.gov/books/NBK5191/box/further_illus-19/)

## Reproducir las pruebas técnicas

Ejecute node test.cjs en el directorio raíz de este repositorio para repetir los casos sintéticos registrados. Se conservan las entradas, los resultados esperados y las tolerancias originales. Las pruebas técnicas no constituyen validación clínica.

```sh
node test.cjs
```

tool.json contiene las fuentes, la edición y el alcance de la revisión. examples.json conserva las entradas y los resultados esperados de los casos sintéticos; results.json registra los resultados obtenidos.

[Ficha y referencias](../tool.json) · [Código JavaScript](../calculator.js) · [Casos de referencia](../examples.json) · [results.json](../results.json)

## Revisión y condiciones de uso

No se ha realizado una revisión clínica independiente.

Esta interfaz es una traducción de elaboración propia, no una edición oficial o certificada. No se han realizado la revisión clínica independiente, la revisión lingüística profesional ni la autorización de derechos de los instrumentos.

Resultado de la fórmula o clasificación. La interpretación, la conducta y la aplicabilidad dependen de la evaluación profesional y de la fuente seleccionada.

## Licencia y atribución

Apache-2.0 se aplica únicamente al código de ELUCENIA. Los derechos de los instrumentos, publicaciones, traducciones y datos permanecen en manos de sus respectivos titulares. Conserve LICENSE y NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026

## Resultados documentados

La información siguiente conserva las salidas del método para ejemplos sintéticos. No constituye una validación clínica independiente.

### 1

Frecuencia de portadores en la población: 1 en 26

| Detalles del resultado | |
| --- | --- |
| Frecuencia del alelo (q) | 2,00% |
| Frecuencia de portadores (2pq) | 3,92% (1 en 26) |
| Riesgo de la pareja por embarazo | 0,038% |


### 2

Frecuencia de portadores en la población: 1 en 26

| Detalles del resultado | |
| --- | --- |
| Frecuencia del alelo (q) | 2,00% |
| Frecuencia de portadores (2pq) | 3,92% (1 en 26) |
| Riesgo de la pareja por embarazo | 0,980% |


### 3

Frecuencia de portadores en la población: 1 en 26

| Detalles del resultado | |
| --- | --- |
| Frecuencia del alelo (q) | 2,00% |
| Frecuencia de portadores (2pq) | 3,92% (1 en 26) |
| Riesgo de la pareja por embarazo | 0,653% |


### 4

Frecuencia de portadores en la población: 1 en 51

| Detalles del resultado | |
| --- | --- |
| Frecuencia del alelo (q) | 1,00% |
| Frecuencia de portadores (2pq) | 1,98% (1 en 51) |
| Riesgo de la pareja por embarazo | 25,000% |


### 5

Frecuencia de portadores en la población: 1 en 51

| Detalles del resultado | |
| --- | --- |
| Frecuencia del alelo (q) | 1,00% |
| Frecuencia de portadores (2pq) | 1,98% (1 en 51) |
| Riesgo de la pareja por embarazo | 0,010% |

