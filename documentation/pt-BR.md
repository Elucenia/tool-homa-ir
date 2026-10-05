<!-- ELUCENIA technical documentation · homa-ir · pt-BR · no clinical/professional/rights approval -->

# HOMA-IR e HOMA-β

[condições, fontes e permissões](https://elucenia.org/pt-br/ferramentas/homa-ir)

## Como usar

Use a ferramenta no portal ou abra index.html em um servidor HTTP local. Selecione o idioma, preencha os campos e calcule.

## Entradas e unidades

### Glicemia de jejum

`glicemia`

mg/dL · intervalo: 40–400

### Insulina de jejum

`insulina`

µU/mL · intervalo: 0,5–300

## Edição do método

HOMA 1/Matthews 1985:IRglicose×insulina/22,5; beta 20 insulina/(glicose−3,5); sem HOMA 2

## Fórmula documentada

HOMA-IR = insulina (µU/mL) × glicemia (mmol/L) ÷ 22,5.

HOMA-β = 20 × insulina (µU/mL) ÷ \[glicemia (mmol/L) − 3,5\] (%).

Glicemia em mmol/L = mg/dL ÷ 18.

## Limites e população

O HOMA depende de concentrações basais em jejum e da interação homeostática entre glicose e insulina. O artigo original reconhece baixa precisão das estimativas. Fórmulas simplificadas HOMA1, modelo HOMA2 e pontos de corte populacionais não são intercambiáveis; o resultado não confirma diagnóstico individual de resistência à insulina.

## Referências

- [Matthews DR et al. Homeostasis model assessment: insulin resistance and β-cell function from fasting plasma glucose and insulin concentrations in man. Diabetologia, 1985.](https://doi.org/10.1007/BF00280883)

- [Geloneze B et al. HOMA1-IR and HOMA2-IR indexes in identifying insulin resistance and metabolic syndrome: Brazilian Metabolic Syndrome Study (BRAMS). Arq Bras Endocrinol Metabol, 2009.](https://doi.org/10.1590/S0004-27302009000200020)

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
