<!-- ELUCENIA technical documentation · homa-ir · de · no clinical/professional/rights approval -->

# HOMA-IR und HOMA-β

[Bedingungen, Quellen und Berechtigungen](https://elucenia.org/de/werkzeuge/homa-ir)

## Verwendung

Verwenden Sie das Werkzeug im Portal oder öffnen Sie index.html über einen lokalen HTTP-Server. Wählen Sie die Sprache, füllen Sie die Felder aus und berechnen Sie das Ergebnis.

## Eingaben und Einheiten

### Nüchternblutzucker

`glicemia`

mg/dL · Bereich: 40–400

### Nüchterninsulin

`insulina`

µU/mL · Bereich: 0,5–300

## Fassung der Methode

HOMA 1/Matthews 1985: IR Glukose×Insulin/22,5; Beta 20 Insulin/(Glukose−3,5); ohne HOMA 2

## Dokumentierte Formel

HOMA-IR = Insulin (µU/mL) × Glukose (mmol/L) ÷ 22,5.

HOMA-β = 20 × Insulin (µU/mL) ÷ \[Glukose (mmol/L) − 3,5\] (%).

Glukose in mmol/L = mg/dL ÷ 18.

## Grenzen und Population

HOMA hängt von basalen Nüchternkonzentrationen und der homöostatischen Wechselwirkung von Glukose und Insulin ab. Der Originalartikel erkennt eine geringe Schätzpräzision an. Vereinfachte HOMA1-Formeln, HOMA2-Modell und populationsbezogene Schwellen sind nicht austauschbar; das Ergebnis bestätigt keine individuelle Insulinresistenzdiagnose.

## Referenzen

- [Matthews DR et al. Homeostasis model assessment: insulin resistance and β-cell function from fasting plasma glucose and insulin concentrations in man. Diabetologia, 1985.](https://doi.org/10.1007/BF00280883)

- [Geloneze B et al. HOMA1-IR and HOMA2-IR indexes in identifying insulin resistance and metabolic syndrome: Brazilian Metabolic Syndrome Study (BRAMS). Arq Bras Endocrinol Metabol, 2009.](https://doi.org/10.1590/S0004-27302009000200020)

## Technische Tests reproduzieren

Führen Sie node test.cjs im Stammverzeichnis dieses Repositorys aus, um die dokumentierten synthetischen Fälle zu wiederholen. Ursprüngliche Eingaben, erwartete Ergebnisse und Toleranzen bleiben erhalten. Technische Tests stellen keine klinische Validierung dar.

```sh
node test.cjs
```

tool.json enthält Quellen, Ausgabe und Umfang der Überprüfung. examples.json bewahrt die synthetischen Eingaben und erwarteten Ergebnisse; results.json dokumentiert die tatsächlich erhaltenen Ergebnisse.

[Eintrag und Referenzen](../tool.json) · [JavaScript-Code](../calculator.js) · [Referenzfälle](../examples.json) · [results.json](../results.json)

## Überprüfung und Nutzungsbedingungen

Eine unabhängige klinische Prüfung wurde nicht durchgeführt.

Diese Benutzeroberfläche ist eine selbst erstellte Übersetzung und keine offizielle oder zertifizierte Ausgabe. Eine unabhängige klinische Überprüfung, eine professionelle sprachliche Prüfung und eine Klärung der Rechte an den Instrumenten wurden nicht durchgeführt.

Ergebnis der Formel oder Klassifikation. Interpretation, Vorgehen und Anwendbarkeit hängen von der fachlichen Beurteilung und der ausgewählten Quelle ab.

## Lizenz und Urheberangaben

Apache-2.0 gilt nur für den ELUCENIA-Code. Die Rechte an Instrumenten, Veröffentlichungen, Übersetzungen und Daten verbleiben bei den jeweiligen Rechteinhabern. Bewahren Sie LICENSE und NOTICE auf.

ELUCENIA · Felipe Guedes · Copyright © 2026
