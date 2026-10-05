<!-- ELUCENIA technical documentation · homa-ir · zh · no clinical/professional/rights approval -->

# HOMA-IR 与 HOMA-β

[条件、来源与许可](https://elucenia.org/zh/tools/homa-ir)

## 使用方法

在门户中使用工具，或通过本地 HTTP 服务器打开 index.html。选择语言，填写各字段，然后计算。

## 输入与单位

### 空腹血糖

`glicemia`

mg/dL · 范围: 40–400

### 空腹胰岛素

`insulina`

µU/mL · 范围: 0.5–300

## 方法版本

HOMA 1/Matthews 1985：IR血糖×胰岛素/22.5；β 20胰岛素/(血糖−3.5)；不含HOMA 2

## 已记录的公式

HOMA-IR = 胰岛素 (µU/mL) × 血糖 (mmol/L) ÷ 22.5.

HOMA-β = 20 × 胰岛素 (µU/mL) ÷ \[血糖 (mmol/L) − 3.5\] (%).

血糖mmol/L = mg/dL ÷ 18.

## 限制与适用人群

HOMA依赖空腹基础浓度及葡萄糖与胰岛素之间的稳态相互作用。原始文章承认估计的精度较低。简化HOMA1公式、HOMA2模型和人群阈值不可互换；结果不能确认个体的胰岛素抵抗诊断。

## 参考文献

- [Matthews DR et al. Homeostasis model assessment: insulin resistance and β-cell function from fasting plasma glucose and insulin concentrations in man. Diabetologia, 1985.](https://doi.org/10.1007/BF00280883)

- [Geloneze B et al. HOMA1-IR and HOMA2-IR indexes in identifying insulin resistance and metabolic syndrome: Brazilian Metabolic Syndrome Study (BRAMS). Arq Bras Endocrinol Metabol, 2009.](https://doi.org/10.1590/S0004-27302009000200020)

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
