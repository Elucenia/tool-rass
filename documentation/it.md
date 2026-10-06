<!-- ELUCENIA technical documentation · rass · it · no clinical/professional/rights approval -->

# Scala di agitazione e sedazione di Richmond (RASS)

[condizioni, fonti e autorizzazioni](https://elucenia.org/it/strumenti/rass)

## Come usare

Usi lo strumento nel portale oppure apra index.html tramite un server HTTP locale. Selezioni la lingua, compili i campi ed esegua il calcolo.

## Dati di ingresso e unità

### Livello osservato

`rass`

- `0` — 0 · Vigile e calmo
- `1` — +1 · Irrequieto: ansioso, movimenti non aggressivi
- `2` — +2 · Agitato: frequenti movimenti senza scopo, contrasta il ventilatore
- `3` — +3 · Molto agitato: tira o rimuove tubi e cateteri; aggressivo
- `4` — +4 · Combattivo: violento, pericolo immediato per il personale
- `-1` — −1 · Sonnolento: si sveglia alla voce e mantiene il contatto visivo per più di 10 s
- `-2` — −2 · Sedazione lieve: si sveglia alla voce, contatto visivo per meno di 10 s
- `-3` — −3 · Sedazione moderata: movimento o apertura degli occhi alla voce, senza contatto visivo
- `-4` — −4 · Sedazione profonda: nessuna risposta alla voce; movimento allo stimolo fisico
- `-5` — −5 · Non risvegliabile: nessuna risposta alla voce né allo stimolo fisico

## Edizione del metodo

RASS/Sessler 2002; Ely 2003: −5 a +4, osservazione→voce→stimolo fisico

## Formula documentata

Valutazione in 3 passi: (1) osservare per 30 s (0 a +4); (2) se non vigile, chiamare per nome e chiedere di guardarvi (−1 a −3); (3) senza risposta alla voce, stimolare muovendo la spalla o sfregando lo sterno (−4 a −5).

## Limiti e popolazione

La RASS del 2002 è stata studiata per agitazione e sedazione negli adulti in terapia intensiva, con e senza ventilazione o sedativi, e ha coinvolto valutatori formati. Il risultato dipende da osservazione e applicazione appropriate; da solo non è una diagnosi di delirium né una prescrizione della dose di sedativo. L’uso pediatrico e i protocolli terapeutici richiedono fonti proprie.

## Riferimenti

- [Sessler CN et al. The Richmond Agitation-Sedation Scale: validity and reliability in adult intensive care unit patients. Am J Respir Crit Care Med, 2002.](https://doi.org/10.1164/rccm.2107138)

- [Ely EW et al. Monitoring sedation status over time in ICU patients: reliability and validity of the Richmond Agitation-Sedation Scale (RASS). JAMA, 2003.](https://doi.org/10.1001/jama.289.22.2983)

- [Devlin JW et al. Clinical practice guidelines for the prevention and management of pain, agitation/sedation, delirium, immobility, and sleep disruption in adult patients in the ICU. Crit Care Med, 2018.](https://doi.org/10.1097/CCM.0000000000003299)

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

## Risultati documentati

Le informazioni seguenti conservano gli output del metodo per esempi sintetici. Non costituiscono una validazione clinica indipendente.

### 1

Sedazione profonda o coma (RASS −4 a −5)

Rivalutare la necessità di sedazione profonda; non è possibile valutare il delirium (CAM-ICU).


### 2

Sedazione moderata (RASS −3)

Al di sopra dell’intervallo abituale di sedazione lieve: considerare di ridurre la sedazione se non vi è indicazione per una sedazione profonda.


### 3

Sedazione lieve fino ad allerta e tranquillo (RASS −2 a 0)

Intervallo obiettivo abituale della sedazione lieve (PADIS 2018). Valutare il delirium con il CAM-ICU.


### 4

Sedazione lieve fino ad allerta e tranquillo (RASS −2 a 0)

Intervallo obiettivo abituale della sedazione lieve (PADIS 2018). Valutare il delirium con il CAM-ICU.


### 5

Irrequieto (RASS +1)

Cercare le cause: dolore, ipossia, vescica piena, astinenza, delirium.


### 6

Agitato fino a combativo (RASS +2 a +4)

Garantire la sicurezza del paziente e dei dispositivi; trattare la causa e considerare la sedazione.

