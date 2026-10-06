<!-- ELUCENIA technical documentation · rass · de · no clinical/professional/rights approval -->

# Richmond-Agitations-Sedierungs-Skala (RASS)

[Bedingungen, Quellen und Berechtigungen](https://elucenia.org/de/werkzeuge/rass)

## Verwendung

Verwenden Sie das Werkzeug im Portal oder öffnen Sie index.html über einen lokalen HTTP-Server. Wählen Sie die Sprache, füllen Sie die Felder aus und berechnen Sie das Ergebnis.

## Eingaben und Einheiten

### Beobachteter Zustand

`rass`

- `0` — 0 · Wach und ruhig
- `1` — +1 · Unruhig: ängstlich, nicht aggressive Bewegungen
- `2` — +2 · Agitiert: häufige ziellose Bewegungen, kämpft gegen das Beatmungsgerät
- `3` — +3 · Stark agitiert: zieht an Schläuchen und Kathetern oder entfernt sie; aggressiv
- `4` — +4 · Streitbar: gewalttätig, unmittelbare Gefahr für das Personal
- `-1` — −1 · Schläfrig: erwacht auf Ansprache und hält länger als 10 s Blickkontakt
- `-2` — −2 · Leichte Sedierung: erwacht auf Ansprache, Blickkontakt kürzer als 10 s
- `-3` — −3 · Mäßige Sedierung: Bewegung oder Augenöffnung auf Ansprache, kein Blickkontakt
- `-4` — −4 · Tiefe Sedierung: keine Reaktion auf Ansprache; Bewegung auf körperliche Stimulation
- `-5` — −5 · Nicht erweckbar: keine Reaktion auf Ansprache oder körperliche Stimulation

## Fassung der Methode

RASS/Sessler 2002; Ely 2003: −5 bis +4, Beobachtung→Stimme→körperlicher Reiz

## Dokumentierte Formel

Beurteilung in 3 Schritten: (1) 30 s beobachten (0 bis +4); (2) bei fehlender Wachheit mit Namen ansprechen und bitten, Sie anzusehen (−1 bis −3); (3) ohne Reaktion auf die Stimme durch Schulterschütteln oder Sternumreiben körperlich stimulieren (−4 bis −5).

## Grenzen und Population

RASS von 2002 wurde für Agitation und Sedierung bei Erwachsenen auf Intensivstationen mit und ohne Beatmung oder Sedativa und mit geschulten Beurteilenden untersucht. Das Ergebnis hängt von angemessener Beobachtung und Anwendung ab; es ist allein weder Delirdiagnose noch Sedativadosisverordnung. Pädiatrische Anwendung und Behandlungsprotokolle benötigen eigene Quellen.

## Referenzen

- [Sessler CN et al. The Richmond Agitation-Sedation Scale: validity and reliability in adult intensive care unit patients. Am J Respir Crit Care Med, 2002.](https://doi.org/10.1164/rccm.2107138)

- [Ely EW et al. Monitoring sedation status over time in ICU patients: reliability and validity of the Richmond Agitation-Sedation Scale (RASS). JAMA, 2003.](https://doi.org/10.1001/jama.289.22.2983)

- [Devlin JW et al. Clinical practice guidelines for the prevention and management of pain, agitation/sedation, delirium, immobility, and sleep disruption in adult patients in the ICU. Crit Care Med, 2018.](https://doi.org/10.1097/CCM.0000000000003299)

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

## Dokumentierte Ergebnisse

Die folgenden Angaben bewahren die Ausgaben der Methode für synthetische Beispiele. Sie stellen keine unabhängige klinische Validierung dar.

### 1

Tiefe Sedierung oder Koma (RASS −4 bis −5)

Die Notwendigkeit einer tiefen Sedierung neu bewerten; ein Delir kann nicht beurteilt werden (CAM-ICU).


### 2

Mäßige Sedierung (RASS −3)

Oberhalb des üblichen Bereichs der leichten Sedierung: Erwägen Sie eine Reduktion der Sedierung, wenn keine Indikation für eine tiefe Sedierung besteht.


### 3

Leichte Sedierung bis wach und ruhig (RASS −2 bis 0)

Üblicher Zielbereich für leichte Sedierung (PADIS 2018). Beurteilen Sie ein Delir mit dem CAM-ICU.


### 4

Leichte Sedierung bis wach und ruhig (RASS −2 bis 0)

Üblicher Zielbereich für leichte Sedierung (PADIS 2018). Beurteilen Sie ein Delir mit dem CAM-ICU.


### 5

Unruhig (RASS +1)

Suchen Sie nach Ursachen: Schmerzen, Hypoxie, volle Blase, Entzug, Delir.


### 6

Agitiert bis kämpferisch (RASS +2 bis +4)

Gewährleisten Sie die Sicherheit des Patienten und der Geräte; behandeln Sie die Ursache und erwägen Sie eine Sedierung.

