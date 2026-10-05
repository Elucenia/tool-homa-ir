<!-- ELUCENIA technical documentation · homa-ir · fr · no clinical/professional/rights approval -->

# HOMA-IR et HOMA-β

[conditions, sources et autorisations](https://elucenia.org/fr/outils/homa-ir)

## Mode d’emploi

Utilisez l’outil sur le portail ou ouvrez index.html via un serveur HTTP local. Sélectionnez la langue, remplissez les champs et lancez le calcul.

## Données d’entrée et unités

### Glycémie à jeun

`glicemia`

mg/dL · intervalle: 40–400

### Insulinémie à jeun

`insulina`

µU/mL · intervalle: 0,5–300

## Édition de la méthode

HOMA 1/Matthews 1985 : IR glucose×insuline/22,5 ; bêta 20 insuline/(glucose−3,5) ; sans HOMA 2

## Formule documentée

HOMA-IR = insuline (µU/mL) × glycémie (mmol/L) ÷ 22,5.

HOMA-β = 20 × insuline (µU/mL) ÷ \[glycémie (mmol/L) − 3,5\] (%).

Glycémie en mmol/L = mg/dL ÷ 18.

## Limites et population

Le HOMA dépend des concentrations basales à jeun et de l’interaction homéostatique entre glucose et insuline. L’article original reconnaît la faible précision des estimations. Les formules simplifiées HOMA1, le modèle HOMA2 et les seuils populationnels ne sont pas interchangeables ; le résultat ne confirme pas un diagnostic individuel d’insulinorésistance.

## Références

- [Matthews DR et al. Homeostasis model assessment: insulin resistance and β-cell function from fasting plasma glucose and insulin concentrations in man. Diabetologia, 1985.](https://doi.org/10.1007/BF00280883)

- [Geloneze B et al. HOMA1-IR and HOMA2-IR indexes in identifying insulin resistance and metabolic syndrome: Brazilian Metabolic Syndrome Study (BRAMS). Arq Bras Endocrinol Metabol, 2009.](https://doi.org/10.1590/S0004-27302009000200020)

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
