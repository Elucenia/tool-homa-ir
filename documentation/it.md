<!-- ELUCENIA technical documentation · homa-ir · it · no clinical/professional/rights approval -->

# HOMA-IR e HOMA-β

[condizioni, fonti e autorizzazioni](https://elucenia.org/it/strumenti/homa-ir)

## Come usare

Usi lo strumento nel portale oppure apra index.html tramite un server HTTP locale. Selezioni la lingua, compili i campi ed esegua il calcolo.

## Dati di ingresso e unità

### Glicemia a digiuno

`glicemia`

mg/dL · intervallo: 40–400

### Insulina a digiuno

`insulina`

µU/mL · intervallo: 0,5–300

## Edizione del metodo

HOMA 1/Matthews 1985: IR glucosio×insulina/22,5; beta 20 insulina/(glucosio−3,5); senza HOMA 2

## Formula documentata

HOMA-IR = insulina (µU/mL) × glicemia (mmol/L) ÷ 22,5.

HOMA-β = 20 × insulina (µU/mL) ÷ \[glicemia (mmol/L) − 3,5\] (%).

Glicemia in mmol/L = mg/dL ÷ 18.

## Limiti e popolazione

L’HOMA dipende dalle concentrazioni basali a digiuno e dall’interazione omeostatica tra glucosio e insulina. L’articolo originale riconosce la bassa precisione delle stime. Formule semplificate HOMA1, modello HOMA2 e soglie di popolazione non sono intercambiabili; il risultato non conferma una diagnosi individuale di insulino-resistenza.

## Riferimenti

- [Matthews DR et al. Homeostasis model assessment: insulin resistance and β-cell function from fasting plasma glucose and insulin concentrations in man. Diabetologia, 1985.](https://doi.org/10.1007/BF00280883)

- [Geloneze B et al. HOMA1-IR and HOMA2-IR indexes in identifying insulin resistance and metabolic syndrome: Brazilian Metabolic Syndrome Study (BRAMS). Arq Bras Endocrinol Metabol, 2009.](https://doi.org/10.1590/S0004-27302009000200020)

## Riprodurre i test tecnici

Esegua node test.cjs nella cartella principale di questo repository per ripetere i casi sintetici registrati. Gli input, i risultati attesi e le tolleranze originali sono conservati. I test tecnici non costituiscono validazione clinica.

```sh
node test.cjs
```

tool.json contiene le fonti, l’edizione e l’ambito della revisione. examples.json conserva gli input e i risultati attesi dei casi sintetici; results.json registra i risultati ottenuti.

[Scheda e riferimenti](../tool.json) · [Codice JavaScript](../calculator.js) · [Casi di riferimento](../examples.json) · [results.json](../results.json)

## Revisione e condizioni d’uso

Non è stata effettuata una revisione clinica indipendente.

Questa interfaccia è una traduzione realizzata dagli autori, non un’edizione ufficiale o certificata. Non sono state eseguite la revisione clinica indipendente, la revisione linguistica professionale né la verifica delle autorizzazioni relative ai diritti sugli strumenti.

Risultato della formula o classificazione. Interpretazione, condotta e applicabilità dipendono dalla valutazione professionale e dalla fonte selezionata.

## Licenza e attribuzione

Apache-2.0 si applica solo al codice di ELUCENIA. I diritti su strumenti, pubblicazioni, traduzioni e dati restano ai rispettivi titolari. Conservi LICENSE e NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026
