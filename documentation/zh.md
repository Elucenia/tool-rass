<!-- ELUCENIA technical documentation · rass · zh · no clinical/professional/rights approval -->

# Richmond 躁动-镇静量表（RASS）

[条件、来源与许可](https://elucenia.org/zh/tools/rass)

## 使用方法

在门户中使用工具，或通过本地 HTTP 服务器打开 index.html。选择语言，填写各字段，然后计算。

## 输入与单位

### 观察到的水平

`rass`

- `0` — 0 · 清醒且平静
- `1` — +1 · 不安：焦虑，动作无攻击性
- `2` — +2 · 躁动：频繁无目的动作，与呼吸机对抗
- `3` — +3 · 非常躁动：拉扯或拔除管路与导管；有攻击性
- `4` — +4 · 好斗：暴力，对工作人员构成立即危险
- `-1` — −1 · 嗜睡：呼唤可唤醒并保持目光接触超过 10 s
- `-2` — −2 · 轻度镇静：呼唤可唤醒，目光接触不足 10 s
- `-3` — −3 · 中度镇静：呼唤后运动或睁眼，但无目光接触
- `-4` — −4 · 深度镇静：对呼唤无反应；对身体刺激有运动
- `-5` — −5 · 无法唤醒：对呼唤和身体刺激均无反应

## 方法版本

RASS/Sessler 2002；Ely 2003：−5至+4，观察→声音→物理刺激

## 已记录的公式

3步评估：（1）观察患者30 s（0至+4）；（2）若不清醒，呼其姓名并请其看向你（−1至−3）；（3）若对声音无反应，摇肩或摩擦胸骨进行物理刺激（−4至−5）。

## 限制与适用人群

2002年的RASS在重症监护室成人中研究躁动和镇静，包括接受或未接受机械通气、使用或未使用镇静药者，并由受过培训的评估者参与。结果依赖适当的观察和实施；它本身既不是谵妄诊断，也不是镇静药剂量处方。儿科应用和治疗方案须有各自的来源支持。

## 参考文献

- [Sessler CN et al. The Richmond Agitation-Sedation Scale: validity and reliability in adult intensive care unit patients. Am J Respir Crit Care Med, 2002.](https://doi.org/10.1164/rccm.2107138)

- [Ely EW et al. Monitoring sedation status over time in ICU patients: reliability and validity of the Richmond Agitation-Sedation Scale (RASS). JAMA, 2003.](https://doi.org/10.1001/jama.289.22.2983)

- [Devlin JW et al. Clinical practice guidelines for the prevention and management of pain, agitation/sedation, delirium, immobility, and sleep disruption in adult patients in the ICU. Crit Care Med, 2018.](https://doi.org/10.1097/CCM.0000000000003299)

## 复现技术测试

在此仓库的根目录中运行 node test.cjs，以重复已记录的合成案例。原始输入、预期结果和容差保持不变。技术测试不构成临床验证。

```sh
node test.cjs
```

tool.json 包含来源、版本和审查范围。examples.json 保留合成输入与预期结果；results.json 记录实际得到的结果。

[记录与参考文献](../tool.json) · [JavaScript代码](../calculator.js) · [参考案例](../examples.json) · [results.json](../results.json)

## 审查与使用条件

尚未开展独立临床审查。

此界面为自主编写的翻译，并非官方或认证版本。尚未完成独立临床审查、专业语言审查或工具权利授权。

公式或分类结果。解释、处理及适用性须结合专业评估和所选来源。

## 许可与署名

Apache-2.0 仅适用于 ELUCENIA 代码。工具、出版物、翻译和数据的权利仍归各自权利人所有。请保留 LICENSE 和 NOTICE。

ELUCENIA · Felipe Guedes · Copyright © 2026
