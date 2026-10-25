# 繁体字ハイライター

日本語テキスト中に残った中文繁体字を検出し、ハイライトするシンプルなツールです。

雑誌・書籍の校正で「繁体字が混入していないか」をチェックする用途を想定しています。

## 使い方

1. [https://yno9.github.io/trahl/](https://yno9.github.io/trahl/) を開く（または `index.html` をブラウザで直接開く）
2. テキストを貼り付けて「ハイライト」を押す
3. 黄色くハイライトされた字が繁体字候補です

ローカルでも使えます（インターネット不要・完全クライアントサイド）。

## 辞書について

- 出典: [OpenCC](https://github.com/BYVoid/OpenCC)（Apache-2.0）
- 使用ファイル: `TSCharacters.txt` / `STCharacters.txt`
- 約 4,180 字の繁体字セット

日本語でも使われる字（例: 國・學・會 など）も含まれるため、ヒットした字は文脈で判断してください。

## ファイル構成

```
index.html      … 本体（UI + ロジック）
trad_chars.js   … OpenCC 由来の繁体字セット
README.md
```

## ライセンス

- ツール本体: GNU Affero General Public License v3.0
- 辞書データ: OpenCC の Apache-2.0 に従う
