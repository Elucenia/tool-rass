<!-- ELUCENIA technical documentation · rass · fr · no clinical/professional/rights approval -->

# Échelle d’agitation et de sédation de Richmond (RASS)

[conditions, sources et autorisations](https://elucenia.org/fr/outils/rass)

## Mode d’emploi

Utilisez l’outil sur le portail ou ouvrez index.html via un serveur HTTP local. Sélectionnez la langue, remplissez les champs et lancez le calcul.

## Données d’entrée et unités

### Niveau observé

`rass`

- `0` — 0 · Alerte et calme
- `1` — +1 · Agité : anxieux, mouvements non agressifs
- `2` — +2 · Agité : mouvements fréquents sans but, lutte contre le ventilateur
- `3` — +3 · Très agité : tire sur les tubes et cathéters ou les retire ; agressif
- `4` — +4 · Combatif : violent, danger immédiat pour l’équipe
- `-1` — −1 · Somnolent : s’éveille à la voix et maintient le contact visuel pendant plus de 10 s
- `-2` — −2 · Sédation légère : s’éveille à la voix, contact visuel pendant moins de 10 s
- `-3` — −3 · Sédation modérée : mouvement ou ouverture des yeux à la voix, sans contact visuel
- `-4` — −4 · Sédation profonde : aucune réponse à la voix ; mouvement à la stimulation physique
- `-5` — −5 · Non éveillable : aucune réponse à la voix ni à la stimulation physique

## Édition de la méthode

RASS/Sessler 2002 ; Ely 2003 : −5 à +4, observation→voix→stimulation physique

## Formule documentée

Évaluation en 3 étapes : (1) observer 30 s (0 à +4) ; (2) s’il n’est pas alerte, appeler le patient par son nom et lui demander de vous regarder (−1 à −3) ; (3) sans réponse à la voix, stimuler en secouant l’épaule ou frottant le sternum (−4 à −5).

## Limites et population

La RASS de 2002 a été étudiée pour l’agitation et la sédation chez des adultes en réanimation, avec ou sans ventilation ou sédatifs, avec des évaluateurs formés. Le résultat dépend d’une observation et d’une application appropriées ; ce n’est ni un diagnostic isolé de delirium ni une prescription de dose de sédatif. L’utilisation pédiatrique et les protocoles thérapeutiques nécessitent leurs propres sources.

## Références

- [Sessler CN et al. The Richmond Agitation-Sedation Scale: validity and reliability in adult intensive care unit patients. Am J Respir Crit Care Med, 2002.](https://doi.org/10.1164/rccm.2107138)

- [Ely EW et al. Monitoring sedation status over time in ICU patients: reliability and validity of the Richmond Agitation-Sedation Scale (RASS). JAMA, 2003.](https://doi.org/10.1001/jama.289.22.2983)

- [Devlin JW et al. Clinical practice guidelines for the prevention and management of pain, agitation/sedation, delirium, immobility, and sleep disruption in adult patients in the ICU. Crit Care Med, 2018.](https://doi.org/10.1097/CCM.0000000000003299)

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

## Résultats documentés

Les informations ci-dessous conservent les sorties de la méthode pour des exemples synthétiques. Elles ne constituent pas une validation clinique indépendante.

### 1

Sédation profonde ou coma (RASS −4 à −5)

Réévaluer la nécessité d’une sédation profonde ; le delirium ne peut pas être évalué (CAM-ICU).


### 2

Sédation modérée (RASS −3)

Au-dessus de l’intervalle habituel de sédation légère : envisagez de réduire la sédation s’il n’y a pas d’indication de sédation profonde.


### 3

Sédation légère à éveillé et calme (RASS −2 à 0)

Plage cible habituelle de sédation légère (PADIS 2018). Évaluez le delirium avec le CAM-ICU.


### 4

Sédation légère à éveillé et calme (RASS −2 à 0)

Plage cible habituelle de sédation légère (PADIS 2018). Évaluez le delirium avec le CAM-ICU.


### 5

Agité (RASS +1)

Recherchez les causes : douleur, hypoxie, vessie pleine, sevrage, delirium.


### 6

Agité à combatif (RASS +2 à +4)

Assurez la sécurité du patient et des dispositifs ; traitez la cause et envisagez une sédation.

