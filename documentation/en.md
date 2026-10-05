<!-- ELUCENIA technical documentation · homa-ir · en · no clinical/professional/rights approval -->

# HOMA-IR and HOMA-β

[conditions, sources and permissions](https://elucenia.org/en/tools/homa-ir)

## How to use

Use the tool in the portal or open index.html through a local HTTP server. Select the language, complete the fields and calculate.

## Inputs and units

### Fasting blood glucose

`glicemia`

mg/dL · range: 40–400

### Fasting insulin

`insulina`

µU/mL · range: 0.5–300

## Method edition

HOMA 1/Matthews 1985: IR glucose×insulin/22.5; beta 20 insulin/(glucose−3.5); excludes HOMA 2

## Documented formula

HOMA-IR = insulin (µU/mL) × glucose (mmol/L) ÷ 22.5.

HOMA-β = 20 × insulin (µU/mL) ÷ \[glucose (mmol/L) − 3.5\] (%).

Glucose in mmol/L = mg/dL ÷ 18.

## Limits and population

HOMA depends on basal fasting concentrations and the homeostatic interaction between glucose and insulin. The original article acknowledges low precision of the estimates. Simplified HOMA1 formulas, the HOMA2 model and population cutoffs are not interchangeable; the result does not confirm an individual diagnosis of insulin resistance.

## References

- [Matthews DR et al. Homeostasis model assessment: insulin resistance and β-cell function from fasting plasma glucose and insulin concentrations in man. Diabetologia, 1985.](https://doi.org/10.1007/BF00280883)

- [Geloneze B et al. HOMA1-IR and HOMA2-IR indexes in identifying insulin resistance and metabolic syndrome: Brazilian Metabolic Syndrome Study (BRAMS). Arq Bras Endocrinol Metabol, 2009.](https://doi.org/10.1590/S0004-27302009000200020)

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
