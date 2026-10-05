<!-- ELUCENIA technical documentation · homa-ir · es · no clinical/professional/rights approval -->

# HOMA-IR y HOMA-β

[condiciones, fuentes y permisos](https://elucenia.org/es/herramientas/homa-ir)

## Cómo usar

Utilice la herramienta en el portal o abra index.html mediante un servidor HTTP local. Seleccione el idioma, complete los campos y calcule.

## Entradas y unidades

### Glucemia en ayunas

`glicemia`

mg/dL · intervalo: 40–400

### Insulina en ayunas

`insulina`

µU/mL · intervalo: 0,5–300

## Edición del método

HOMA 1/Matthews 1985: IR glucosa×insulina/22,5; beta 20 insulina/(glucosa−3,5); no HOMA 2

## Fórmula documentada

HOMA-IR = insulina (µU/mL) × glucemia (mmol/L) ÷ 22,5.

HOMA-β = 20 × insulina (µU/mL) ÷ \[glucemia (mmol/L) − 3,5\] (%).

Glucemia en mmol/L = mg/dL ÷ 18.

## Límites y población

El HOMA depende de concentraciones basales en ayunas y de la interacción homeostática entre glucosa e insulina. El artículo original reconoce la baja precisión de las estimaciones. Las fórmulas simplificadas HOMA1, el modelo HOMA2 y los puntos de corte poblacionales no son intercambiables; el resultado no confirma un diagnóstico individual de resistencia a la insulina.

## Referencias

- [Matthews DR et al. Homeostasis model assessment: insulin resistance and β-cell function from fasting plasma glucose and insulin concentrations in man. Diabetologia, 1985.](https://doi.org/10.1007/BF00280883)

- [Geloneze B et al. HOMA1-IR and HOMA2-IR indexes in identifying insulin resistance and metabolic syndrome: Brazilian Metabolic Syndrome Study (BRAMS). Arq Bras Endocrinol Metabol, 2009.](https://doi.org/10.1590/S0004-27302009000200020)

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
