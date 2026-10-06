<!-- ELUCENIA technical documentation · homa-ir · ja · no clinical/professional/rights approval -->

# HOMA-IR・HOMA-β

[条件・出典・許諾](https://elucenia.org/ja/tools/homa-ir)

## 使い方

ポータルでツールを使用するか、ローカルHTTPサーバー経由でindex.htmlを開いてください。言語を選択し、項目を入力して計算してください。

## 入力項目と単位

### 空腹時血糖

`glicemia`

mg/dL · 範囲: 40–400

### 空腹時インスリン

`insulina`

µU/mL · 範囲: 0.5–300

## 方法の版

HOMA 1/Matthews 1985：IR血糖×インスリン/22.5；β 20インスリン/(血糖−3.5)；HOMA 2を含まない

## 記載された計算式

HOMA-IR = インスリン (µU/mL) × 血糖 (mmol/L) ÷ 22.5.

HOMA-β = 20 × インスリン (µU/mL) ÷ \[血糖 (mmol/L) − 3.5\] (%).

血糖mmol/L = mg/dL ÷ 18.

## 限界・対象集団

HOMAは、空腹時の基礎濃度と、グルコース・インスリン間の恒常性の相互作用に依存します。原論文は推定の精度が低いことを認めています。簡略化されたHOMA1の式、HOMA2モデル、集団別の閾値は互換ではありません。結果は個人のインスリン抵抗性の診断を確定するものではありません。

## 参考文献

- [Matthews DR et al. Homeostasis model assessment: insulin resistance and β-cell function from fasting plasma glucose and insulin concentrations in man. Diabetologia, 1985.](https://doi.org/10.1007/BF00280883)

- [Geloneze B et al. HOMA1-IR and HOMA2-IR indexes in identifying insulin resistance and metabolic syndrome: Brazilian Metabolic Syndrome Study (BRAMS). Arq Bras Endocrinol Metabol, 2009.](https://doi.org/10.1590/S0004-27302009000200020)

## 技術テストの再現

このリポジトリのルートディレクトリでnode test.cjsを実行すると、記録された合成ケースを再実行できます。元の入力、期待結果、許容誤差は保持されています。技術テストは臨床的検証を意味しません。

```sh
node test.cjs
```

tool.jsonには出典、版、確認範囲が記録されています。examples.jsonには合成入力と期待結果が保持され、results.jsonには実際に得られた結果が記録されています。

[記録・参考文献](../tool.json) · [JavaScriptコード](../calculator.js) · [参照ケース](../examples.json) · [results.json](../results.json)

## 確認状況と使用条件

独立した臨床レビューは実施されていません。

このインターフェースは独自に作成した翻訳であり、公式版や認証済みの版ではありません。独立した臨床レビュー、専門家による言語レビュー、評価尺度等の権利許諾の確認は実施されていません。

式または分類の結果です。解釈、対応、適用可能性は専門家による評価と選択した出典に依存します。

## ライセンスと帰属表示

Apache-2.0はELUCENIAのコードにのみ適用されます。評価尺度等、出版物、翻訳、データの権利は、それぞれの権利者に帰属します。LICENSEとNOTICEを保持してください。

ELUCENIA · Felipe Guedes · Copyright © 2026

## 記録された結果

以下の情報は、合成例に対する手法の出力を保持したものです。独立した臨床的検証を示すものではありません。

### 1

2,7 まで: BRAMS のカットオフではインスリン抵抗性なし

| 結果の詳細 | |
| --- | --- |
| HOMA-β（β細胞機能） | 133.3% |
| 血糖 | 5.00 mmol/L |


### 2

2,7 まで: BRAMS のカットオフではインスリン抵抗性なし

| 結果の詳細 | |
| --- | --- |
| HOMA-β（β細胞機能） | 270.0% |
| 血糖 | 4.50 mmol/L |


### 3

2,7 を超える: インスリン抵抗性を示唆する（BRAMS のカットオフ）

| 結果の詳細 | |
| --- | --- |
| HOMA-β（β細胞機能） | 145.9% |
| 血糖 | 5.56 mmol/L |

