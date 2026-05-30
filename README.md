# Pulse Cable Simulator

A/B相・COM共通線を含む、24Vパルス長距離ケーブルの簡易シミュレーションHTMLアプリです。

## 使い方

1. GitHub Pagesを有効にします。
   - Repository Settings
   - Pages
   - Source: `Deploy from a branch`
   - Branch: `main` / `/root`
   - Save
2. 数分後、以下のURLで開けます。

```text
https://kouheim1979.github.io/pulse/
```

## 内容

- A相、B相、COM導体の近似モデル
- A-COM容量、B-COM容量、A-B容量
- 導体抵抗
- 出力側ダンピング抵抗
- 入力側直列抵抗
- PLC入力抵抗・入力容量
- 10us入力フィルタ
- ON/OFFしきい値判定
- Plotlyによる波形表示

## 注意

このアプリは厳密なSPICE解析ではなく、設計検討用の近似シミュレーションです。
実機波形との照合では、出力立上り時間、PLC入力容量、ケーブル容量、COM配線、シールド接地条件を調整してください。
