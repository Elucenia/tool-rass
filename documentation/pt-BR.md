<!-- ELUCENIA technical documentation · rass · pt-BR · no clinical/professional/rights approval -->

# Escala de Agitação e Sedação de Richmond (RASS)

[condições, fontes e permissões](https://elucenia.org/pt-br/ferramentas/rass)

## Como usar

Use a ferramenta no portal ou abra index.html em um servidor HTTP local. Selecione o idioma, preencha os campos e calcule.

## Entradas e unidades

### Nível observado

`rass`

- `0` — 0 · Alerta e calmo
- `1` — +1 · Inquieto: ansioso, movimentos não agressivos
- `2` — +2 · Agitado: movimentos frequentes sem propósito, briga com o ventilador
- `3` — +3 · Muito agitado: puxa ou remove tubos e cateteres; agressivo
- `4` — +4 · Combativo: violento, perigo imediato para a equipe
- `-1` — −1 · Sonolento: desperta à voz e mantém contato visual por mais de 10 s
- `-2` — −2 · Sedação leve: desperta à voz, contato visual por menos de 10 s
- `-3` — −3 · Sedação moderada: movimento ou abertura ocular à voz, sem contato visual
- `-4` — −4 · Sedação profunda: sem resposta à voz; movimento ao estímulo físico
- `-5` — −5 · Não despertável: sem resposta à voz nem ao estímulo físico

## Edição do método

RASS/Sessler 2002:Ely 2003:−5 a+4, observação→voz→estímulo físico

## Fórmula documentada

Avaliação em 3 passos: (1) observe o paciente por 30 s (0 a +4); (2) se não estiver alerta, chame-o pelo nome e peça que olhe para você (−1 a −3); (3) sem resposta à voz, estimule fisicamente balançando o ombro ou esfregando o esterno (−4 a −5).

## Limites e população

A RASS de 2002 foi estudada para agitação e sedação em adultos de UTI, com e sem ventilação ou sedativos, e envolveu avaliadores treinados. O resultado depende de observação e aplicação apropriadas; não é, isoladamente, diagnóstico de delirium nem prescrição de dose de sedativo. Uso pediátrico e protocolos de tratamento requerem fontes próprias.

## Referências

- [Sessler CN et al. The Richmond Agitation-Sedation Scale: validity and reliability in adult intensive care unit patients. Am J Respir Crit Care Med, 2002.](https://doi.org/10.1164/rccm.2107138)

- [Ely EW et al. Monitoring sedation status over time in ICU patients: reliability and validity of the Richmond Agitation-Sedation Scale (RASS). JAMA, 2003.](https://doi.org/10.1001/jama.289.22.2983)

- [Devlin JW et al. Clinical practice guidelines for the prevention and management of pain, agitation/sedation, delirium, immobility, and sleep disruption in adult patients in the ICU. Crit Care Med, 2018.](https://doi.org/10.1097/CCM.0000000000003299)

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
