<!-- ELUCENIA technical documentation · rass · es · no clinical/professional/rights approval -->

# Escala de agitación y sedación de Richmond (RASS)

[condiciones, fuentes y permisos](https://elucenia.org/es/herramientas/rass)

## Cómo usar

Utilice la herramienta en el portal o abra index.html mediante un servidor HTTP local. Seleccione el idioma, complete los campos y calcule.

## Entradas y unidades

### Nivel observado

`rass`

- `0` — 0 · Alerta y tranquilo
- `1` — +1 · Inquieto: ansioso, movimientos no agresivos
- `2` — +2 · Agitado: movimientos frecuentes sin finalidad, lucha contra el ventilador
- `3` — +3 · Muy agitado: tira de tubos y catéteres o los retira; agresivo
- `4` — +4 · Combativo: violento, peligro inmediato para el equipo
- `-1` — −1 · Somnoliento: despierta a la voz y mantiene contacto visual durante más de 10 s
- `-2` — −2 · Sedación ligera: despierta a la voz, contacto visual durante menos de 10 s
- `-3` — −3 · Sedación moderada: movimiento o apertura ocular a la voz, sin contacto visual
- `-4` — −4 · Sedación profunda: sin respuesta a la voz; movimiento al estímulo físico
- `-5` — −5 · No despertable: sin respuesta a la voz ni al estímulo físico

## Edición del método

RASS/Sessler 2002; Ely 2003: −5 a +4, observación→voz→estímulo físico

## Fórmula documentada

Evaluación en 3 pasos: (1) observe durante 30 s (0 a +4); (2) si no está alerta, llámelo por su nombre y pida que le mire (−1 a −3); (3) sin respuesta a la voz, estimule moviendo el hombro o frotando el esternón (−4 a −5).

## Límites y población

La RASS de 2002 se estudió para agitación y sedación en adultos de UCI, con y sin ventilación o sedantes, e incluyó evaluadores formados. El resultado depende de una observación y aplicación apropiadas; no es por sí solo un diagnóstico de delirium ni una prescripción de dosis de sedante. El uso pediátrico y los protocolos de tratamiento requieren fuentes propias.

## Referencias

- [Sessler CN et al. The Richmond Agitation-Sedation Scale: validity and reliability in adult intensive care unit patients. Am J Respir Crit Care Med, 2002.](https://doi.org/10.1164/rccm.2107138)

- [Ely EW et al. Monitoring sedation status over time in ICU patients: reliability and validity of the Richmond Agitation-Sedation Scale (RASS). JAMA, 2003.](https://doi.org/10.1001/jama.289.22.2983)

- [Devlin JW et al. Clinical practice guidelines for the prevention and management of pain, agitation/sedation, delirium, immobility, and sleep disruption in adult patients in the ICU. Crit Care Med, 2018.](https://doi.org/10.1097/CCM.0000000000003299)

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

## Resultados documentados

La información siguiente conserva las salidas del método para ejemplos sintéticos. No constituye una validación clínica independiente.

### 1

Sedación profunda o coma (RASS −4 a −5)

Reevalúe la necesidad de sedación profunda; no es posible evaluar el delirium (CAM-ICU).


### 2

Sedación moderada (RASS −3)

Por encima del rango habitual de sedación ligera: considere reducir la sedación si no hay indicación de sedación profunda.


### 3

Sedación ligera a alerta y tranquilo (RASS −2 a 0)

Rango objetivo habitual de sedación ligera (PADIS 2018). Evalúe el delirium con CAM-ICU.


### 4

Sedación ligera a alerta y tranquilo (RASS −2 a 0)

Rango objetivo habitual de sedación ligera (PADIS 2018). Evalúe el delirium con CAM-ICU.


### 5

Inquieto (RASS +1)

Busque causas: dolor, hipoxia, vejiga llena, abstinencia, delirium.


### 6

Agitado hasta combativo (RASS +2 a +4)

Asegure la seguridad del paciente y de los dispositivos; trate la causa y considere la sedación.

