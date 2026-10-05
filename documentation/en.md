<!-- ELUCENIA technical documentation · rass · en · no clinical/professional/rights approval -->

# Richmond Agitation–Sedation Scale (RASS)

[conditions, sources and permissions](https://elucenia.org/en/tools/rass)

## How to use

Use the tool in the portal or open index.html through a local HTTP server. Select the language, complete the fields and calculate.

## Inputs and units

### Observed level

`rass`

- `0` — 0 · Alert and calm
- `1` — +1 · Restless: anxious, non-aggressive movements
- `2` — +2 · Agitated: frequent purposeless movements, fights the ventilator
- `3` — +3 · Very agitated: pulls or removes tubes and catheters; aggressive
- `4` — +4 · Combative: violent, immediate danger to staff
- `-1` — −1 · Drowsy: awakens to voice and maintains eye contact for more than 10 s
- `-2` — −2 · Light sedation: awakens to voice, eye contact for less than 10 s
- `-3` — −3 · Moderate sedation: movement or eye opening to voice, no eye contact
- `-4` — −4 · Deep sedation: no response to voice; movement with physical stimulation
- `-5` — −5 · Unarousable: no response to voice or physical stimulation

## Method edition

RASS/Sessler 2002; Ely 2003: −5 to +4, observation→voice→physical stimulus

## Documented formula

Assessment in 3 steps: (1) observe for 30 s (0 to +4); (2) if not alert, call the patient’s name and ask them to look at you (−1 to −3); (3) if there is no voice response, physically stimulate by shaking the shoulder or rubbing the sternum (−4 to −5).

## Limits and population

The 2002 RASS was studied for agitation and sedation in adult ICU patients, with and without ventilation or sedatives, and involved trained raters. The result depends on appropriate observation and application; alone, it is neither a delirium diagnosis nor a sedative-dose prescription. Pediatric use and treatment protocols require their own sources.

## References

- [Sessler CN et al. The Richmond Agitation-Sedation Scale: validity and reliability in adult intensive care unit patients. Am J Respir Crit Care Med, 2002.](https://doi.org/10.1164/rccm.2107138)

- [Ely EW et al. Monitoring sedation status over time in ICU patients: reliability and validity of the Richmond Agitation-Sedation Scale (RASS). JAMA, 2003.](https://doi.org/10.1001/jama.289.22.2983)

- [Devlin JW et al. Clinical practice guidelines for the prevention and management of pain, agitation/sedation, delirium, immobility, and sleep disruption in adult patients in the ICU. Crit Care Med, 2018.](https://doi.org/10.1097/CCM.0000000000003299)

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
