# masata. — Official Site

音楽家 masata. のアーティストページです。ビルド不要の静的サイト（HTML / CSS / JS）で、GitHub Pages でそのまま公開できます。

## 構成

| ファイル | 役割 |
| --- | --- |
| `index.html` | ページ本体。文章・リリース・ライブ・お知らせ・リンクはすべてここ |
| `css/style.css` | デザイン。色と書体は冒頭の `:root` で一括変更 |
| `js/main.js` | スマホメニュー、スクロール時の表示アニメーション |
| `assets/` | 画像置き場（アーティスト写真、ジャケット、OGP画像など） |

## 内容の書き換え

現在は仮の文章が入っています。`index.html` 内のコメントを目印に書き換えてください。

- **プロフィール**: `PROFILE` セクションの文章と、拠点・ジャンル・活動開始年
- **写真・ジャケット**: `assets/` に画像を置き、コメントアウトされている `<img>` 行を有効にする
- **リリース / ライブ / お知らせ**: `<li>…</li>` をコピーして増減
- **リンク**: `href="#"` を各サービスのURLに、`contact@example.com` を連絡先に変更
- **OGP画像**: `assets/ogp.png`（1200×630px 推奨）を追加

## ローカルで確認

```sh
python3 -m http.server 8000
# http://localhost:8000 を開く
```

## GitHub Pages で公開

1. リポジトリの **Settings → Pages** を開く
2. **Source** を「Deploy from a branch」にし、公開するブランチと `/ (root)` を選んで保存
3. 数分後に `https://<ユーザー名>.github.io/masata/` で公開されます
