# Tea & Trade English

英国ビジネス英語の12機能を、日本語から英語へ整理して学ぶ、音声つきカードデッキです。

## 内容

- 日本語で機能を確認
- 英語フレーズをカードで復習
- 差し替え部分を薄色表示
- ブラウザの `en-GB` 音声を優先して読み上げ
- 上下スクロールでセクション移動
- 横スワイプでランダム移動
- PWA対応：ホーム画面追加・簡易オフライン表示

## ファイル構成

```text
.
├── index.html
├── manifest.webmanifest
├── service-worker.js
└── assets/
    ├── favicon.svg
    ├── icon-192.png
    └── icon-512.png
```

## GitHub Pagesで公開する手順

1. このフォルダの中身をGitHubリポジトリにアップロードします。
2. GitHubの `Settings` → `Pages` を開きます。
3. `Build and deployment` の `Source` を `Deploy from a branch` にします。
4. `Branch` を `main`、フォルダを `/root` にして保存します。
5. 表示されたURLで `index.html` が開ければ完了です。

## 音声について

音声は端末・ブラウザ内蔵のWeb Speech APIを使います。端末に英国英語音声が入っている場合は `en-GB` を優先します。環境によって声質や再生可否が変わります。

## カスタマイズ

カード内容は `index.html` 内の `BOXES` 配列を編集すると変更できます。
