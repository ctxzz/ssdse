# SSDSE（教育用標準データセット）配布

このリポジトリは、独立行政法人統計センターが公開している SSDSE（教育用標準データセット）を、
浜松医科大学 データサイエンス授業の教材として再配布しているものです。

## ファイル一覧

- `SSDSE-B-2026.csv` — 県別推移（47都道府県 × 約110項目 × 12年分、2012〜2023年）
  - 元データ（.xlsx）と同じ構造を維持しています
  - 1行目：項目コード、2行目：日本語列名、3行目以降：データ

## Colab での読み込み方

```python
import pandas as pd
url = 'https://raw.githubusercontent.com/ctxzz/ssdse/main/SSDSE-B-2026.csv'
df = pd.read_csv(url, header=1)
df.head()
```

`header=1` は「2行目（インデックス1）を列名として使う」という指定です。元のSSDSE形式に合わせています。

## 出典

「SSDSE-B-2026 県別推移」（独立行政法人統計センター）
https://www.nstac.go.jp/use/literacy/ssdse/

データの著作権は独立行政法人統計センターに帰属します。
本リポジトリは同センターのサイト利用ルール（**政府標準利用規約 第2.0版に準拠、CC BY 4.0 と互換**）に基づき再配布しています。

サイトポリシー詳細：https://www.nstac.go.jp/info/site-policy/

## ライセンス

- **データ**：独立行政法人統計センターのサイト利用ルール（政府標準利用規約 第2.0版に準拠）。CC BY 4.0 に従っての利用も可能。
- **README 等の解説部分**：CC BY 4.0
