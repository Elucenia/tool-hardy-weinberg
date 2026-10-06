<!-- ELUCENIA technical documentation · hardy-weinberg · zh · no clinical/professional/rights approval -->

# Hardy-Weinberg 平衡

[条件、来源与许可](https://elucenia.org/zh/tools/hardy-weinberg)

## 使用方法

在门户中使用工具，或通过本地 HTTP 服务器打开 index.html。选择语言，填写各字段，然后计算。

## 输入与单位

### 疾病频率：每多少人中有 1 人患病

`incid`

出生人数 · 范围: 100–1000000

### 伴侣 1

`p1`

- `pop` — 一般人群
- `port` — 已确认携带者
- `irmao` — 患病者未受累的兄弟姐妹

### 伴侣 2

`p2`

- `pop` — 一般人群
- `port` — 已确认携带者
- `irmao` — 患病者未受累的兄弟姐妹

## 方法版本

Hardy–Weinberg 1908：p²+2pq+q²；常染色体隐性遗传；未患病同胞2/3；夫妇风险×1/4

## 已记录的公式

平衡时：p² + 2pq + q² = 1，q为致病等位基因频率，p = 1 − q。

发病率 = q²，因此q = √发病率。

携带者（杂合子）频率 = 2pq（q较小时≈ 2q）。

各配偶携带概率：一般人群 = 2pq；确诊携带者 = 1；患病者的未患病兄弟姐妹 = 2/3。

每次妊娠风险 = P(配偶1携带) × P(配偶2携带) × 1/4。

## 限制与适用人群

群体计算假定常染色体上的一个双等位基因位点处于 Hardy–Weinberg 平衡；随机交配和理想状态下非常大的群体是前提，并非计算结果。将 q² 作为患病频率要求符合所考虑的隐性遗传模型。25% 的家族风险假定父母双方均为携带者；未患病同胞的 2/3 是该情境下的条件概率。不要将这些关系用于所有遗传病，也不要将其解释为个体诊断。

## 参考文献

- [Hardy GH. Mendelian proportions in a mixed population. Science, 1908.](https://doi.org/10.1126/science.28.706.49)

- [Mayo O. A century of Hardy-Weinberg equilibrium. Twin Res Hum Genet, 2008.](https://doi.org/10.1375/twin.11.3.249)

- [GeneReviews carrier box,revised2016](https://www.ncbi.nlm.nih.gov/books/NBK5191/box/further_illus-19/)

## 复现技术测试

在此仓库的根目录中运行 node test.cjs，以重复已记录的合成案例。原始输入、预期结果和容差保持不变。技术测试不构成临床验证。

```sh
node test.cjs
```

tool.json 包含来源、版本和审查范围。examples.json 保留合成输入与预期结果；results.json 记录实际得到的结果。

[记录与参考文献](../tool.json) · [JavaScript代码](../calculator.js) · [参考案例](../examples.json) · [results.json](../results.json)

## 审查与使用条件

尚未开展独立临床审查。

此界面为自主编写的翻译，并非官方或认证版本。尚未完成独立临床审查、专业语言审查或工具权利授权。

公式或分类结果。解释、处理及适用性须结合专业评估和所选来源。

## 许可与署名

Apache-2.0 仅适用于 ELUCENIA 代码。工具、出版物、翻译和数据的权利仍归各自权利人所有。请保留 LICENSE 和 NOTICE。

ELUCENIA · Felipe Guedes · Copyright © 2026

## 已记录的结果

以下信息保留该方法对合成示例的输出，不构成独立的临床验证。

### 1

人群中的携带者频率：1/26

| 结果详情 | |
| --- | --- |
| 等位基因频率（q） | 2.00% |
| 携带者频率（2pq） | 3.92%（1/26） |
| 每次妊娠的夫妻风险 | 0.038% |


### 2

人群中的携带者频率：1/26

| 结果详情 | |
| --- | --- |
| 等位基因频率（q） | 2.00% |
| 携带者频率（2pq） | 3.92%（1/26） |
| 每次妊娠的夫妻风险 | 0.980% |


### 3

人群中的携带者频率：1/26

| 结果详情 | |
| --- | --- |
| 等位基因频率（q） | 2.00% |
| 携带者频率（2pq） | 3.92%（1/26） |
| 每次妊娠的夫妻风险 | 0.653% |


### 4

人群中的携带者频率：1/51

| 结果详情 | |
| --- | --- |
| 等位基因频率（q） | 1.00% |
| 携带者频率（2pq） | 1.98%（1/51） |
| 每次妊娠的夫妻风险 | 25.000% |


### 5

人群中的携带者频率：1/51

| 结果详情 | |
| --- | --- |
| 等位基因频率（q） | 1.00% |
| 携带者频率（2pq） | 1.98%（1/51） |
| 每次妊娠的夫妻风险 | 0.010% |

