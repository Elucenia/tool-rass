<!-- ELUCENIA technical documentation · rass · ja · no clinical/professional/rights approval -->

# Richmond興奮・鎮静スケール（RASS）

[条件・出典・許諾](https://elucenia.org/ja/tools/rass)

## 使い方

ポータルでツールを使用するか、ローカルHTTPサーバー経由でindex.htmlを開いてください。言語を選択し、項目を入力して計算してください。

## 入力項目と単位

### 観察されたレベル

`rass`

- `0` — 0 · 覚醒し穏やか
- `1` — +1 · 落ち着かない：不安、非攻撃的な動き
- `2` — +2 · 興奮：頻繁で無目的な動き、人工呼吸器と同調しない
- `3` — +3 · 非常に興奮：チューブ・カテーテルを引っ張る、抜去する；攻撃的
- `4` — +4 · 好戦的：暴力的、スタッフに差し迫った危険
- `-1` — −1 · 傾眠：呼びかけで覚醒し、10 sを超えて視線を合わせる
- `-2` — −2 · 浅い鎮静：呼びかけで覚醒、視線の合う時間は10 s未満
- `-3` — −3 · 中等度の鎮静：呼びかけで動くか開眼するが視線は合わない
- `-4` — −4 · 深い鎮静：呼びかけに反応なし、身体刺激で動く
- `-5` — −5 · 覚醒不能：呼びかけにも身体刺激にも反応なし

## 方法の版

RASS/Sessler 2002、Ely 2003：−5～+4、観察→呼びかけ→身体刺激

## 記載された計算式

3段階の評価：（1）30 s観察（0～+4）、（2）覚醒していなければ名前で呼び、こちらを見るよう指示（−1～−3）、（3）声に反応しなければ肩を揺するか胸骨を擦って刺激（−4～−5）。

## 限界・対象集団

2002年のRASSは、人工呼吸や鎮静薬の使用の有無を問わず、ICUの成人の興奮・鎮静について研究され、訓練を受けた評価者が参加しました。結果は適切な観察と実施に依存します。単独ではせん妄の診断にも鎮静薬の用量処方にもなりません。小児での使用と治療プロトコルには、それぞれの出典が必要です。

## 参考文献

- [Sessler CN et al. The Richmond Agitation-Sedation Scale: validity and reliability in adult intensive care unit patients. Am J Respir Crit Care Med, 2002.](https://doi.org/10.1164/rccm.2107138)

- [Ely EW et al. Monitoring sedation status over time in ICU patients: reliability and validity of the Richmond Agitation-Sedation Scale (RASS). JAMA, 2003.](https://doi.org/10.1001/jama.289.22.2983)

- [Devlin JW et al. Clinical practice guidelines for the prevention and management of pain, agitation/sedation, delirium, immobility, and sleep disruption in adult patients in the ICU. Crit Care Med, 2018.](https://doi.org/10.1097/CCM.0000000000003299)

## 技術テストの再現

このリポジトリのルートディレクトリでnode test.cjsを実行すると、記録された合成ケースを再実行できます。元の入力、期待結果、許容誤差は保持されています。技術テストは臨床的検証を意味しません。

```sh
node test.cjs
```

tool.jsonには出典、版、確認範囲が記録されています。examples.jsonには合成入力と期待結果が保持され、results.jsonには実際に得られた結果が記録されています。

[記録・参考文献](../tool.json) · [JavaScriptコード](../calculator.js) · [参照ケース](../examples.json) · [results.json](../results.json)

## 確認状況と使用条件

独立した臨床レビューは実施されていません。

このインターフェースは独自に作成した翻訳であり、公式版や認証済みの版ではありません。独立した臨床レビュー、専門家による言語レビュー、評価尺度等の権利許諾の確認は実施されていません。

式または分類の結果です。解釈、対応、適用可能性は専門家による評価と選択した出典に依存します。

## ライセンスと帰属表示

Apache-2.0はELUCENIAのコードにのみ適用されます。評価尺度等、出版物、翻訳、データの権利は、それぞれの権利者に帰属します。LICENSEとNOTICEを保持してください。

ELUCENIA · Felipe Guedes · Copyright © 2026

## 記録された結果

以下の情報は、合成例に対する手法の出力を保持したものです。独立した臨床的検証を示すものではありません。

### 1

深鎮静または昏睡（RASS −4～−5）

深鎮静の必要性を再評価する；せん妄（CAM-ICU）は評価できない。


### 2

中等度鎮静（RASS −3）

通常の軽度鎮静の範囲を上回る：深鎮静の適応がなければ、鎮静の減量を考慮する。


### 3

軽度鎮静から覚醒して落ち着いている状態（RASS −2〜0）

軽度鎮静の通常の目標範囲（PADIS 2018）。CAM-ICUでせん妄を評価する。


### 4

軽度鎮静から覚醒して落ち着いている状態（RASS −2〜0）

軽度鎮静の通常の目標範囲（PADIS 2018）。CAM-ICUでせん妄を評価する。


### 5

落ち着きがない（RASS +1）

原因を探す：痛み、低酸素、膀胱充満、離脱、せん妄。


### 6

興奮から攻撃的（RASS +2〜+4）

患者と機器の安全を確保し、原因を治療し、鎮静を検討する。

