# 2026-08-20 drill down

デモ画面

https://saitotsutomu.github.io/drill-down/

## 概要

ユーザーの行動履歴や業務プロセスなどのフローデータをブラウザ上で可視化し、直感的な操作でフィルタリング・分析を行うアプリです。

ノードやエッジをダブルクリックすると、対象を通るフローだけに絞り込みます。再度ダブルクリックすると解除されます。

## ローカルで実行

下記を実行して `http://localhost:8000/` を開いてください。

```sh
python3 -m http.server 8000
```

## GitHub Pages で公開する

元のリポジトリの`dist/`以下をコピーする
このリポジトリは静的ファイル構成なので、ビルド不要でそのまま公開できます。

1. GitHubにpushする

```bash
git add .
git commit -m "Prepare for GitHub Pages"
git push origin master
```

2. GitHub のリポジトリ画面で Settings > Pages を開く
3. Build and deployment の Source を Deploy from a branch にする
4. Branch を master、Folder を /(root) にして Save
5. 数十秒〜数分待つと公開 URL が表示される

公開 URL の例:

```text
https://<ユーザー名>.github.io/drill-down/
```

更新時は master に push するだけで再デプロイされます。

## 主なファイル構成

- index.html: メイン画面
- assets/: CSSとJS
