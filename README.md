# 夜想の魔剣 ─ Nocturne Blade

スマートフォンの縦画面・親指1本で遊べる2Dアクションゲームです。
ビルド不要の静的ファイルだけで動くので、どこに置いてもURLを開くだけで遊べます。

## 同梱ファイル

| ファイル | 役割 |
| --- | --- |
| `index.html` | ゲーム本体（HTML / CSS / JavaScript をすべて含む） |
| `manifest.webmanifest` | ホーム画面に追加したときの名前・全画面表示・縦固定の設定 |
| `icon-192.png` / `icon-512.png` | Android のホーム画面アイコン |
| `apple-touch-icon.png` | iPhone のホーム画面アイコン |
| `.nojekyll` | GitHub Pages で余計な変換をさせないための空ファイル |

※ `index.html` だけでもゲームは完全に動きます。ほかのファイルはホーム画面追加用です。

## GitHub Pages で公開する手順（ブラウザだけで完結）

1. GitHub にログインし、右上の「+」→「New repository」。
   名前は例えば `nocturne-blade`、**Public** を選んで「Create repository」。
2. 作成直後の画面で「uploading an existing file」をクリック。
3. このフォルダの中身（`index.html` など全ファイル）をまとめてドラッグ＆ドロップし、「Commit changes」。
   - `.nojekyll` は隠しファイルなので見えない場合がありますが、なくても動作します。
4. リポジトリの「Settings」→ 左メニュー「Pages」。
   「Branch」を `main`、フォルダを `/ (root)` にして「Save」。
5. 1〜2分待つと、同じ画面に公開URLが表示されます。
   例：`https://あなたのユーザー名.github.io/nocturne-blade/`

このURLを友達に送れば、アカウント登録なしでスマホからすぐ遊べます。
ゲームオーバー／クリア画面の「友達に送る」ボタンからも、LINE などの共有シートでURLを送れます。

### さらに手軽な方法：Netlify Drop

https://app.netlify.com/drop を開き、このフォルダごとドラッグ＆ドロップするだけで公開URLが発行されます。
（ログインせずに作ったURLは一定時間で消えるため、残したい場合は無料アカウントで保存してください）

## スマホでの遊び方のコツ

- **iPhone（Safari）**：共有ボタン →「ホーム画面に追加」で、アドレスバーのない全画面で遊べます。
- **Android（Chrome）**：START を押すと自動で全画面になります。メニュー →「ホーム画面に追加」も可能です。
- **音が出ないとき（iPhone）**：本体の消音スイッチ（マナーモード）がオンだと効果音が鳴りません。
- 画面右上のスピーカーボタンで効果音のオン／オフを切り替えられます。

## 動作環境

- iOS Safari 13 以降 / Android Chrome 80 以降（Pointer Events と Canvas 2D に対応したブラウザ）
- PC ブラウザでも、マウスのドラッグ・クリックで操作できます（画面中央に縦長で表示されます）。
- 処理が重い端末では、描画解像度を自動で下げてなめらかさを保ちます。
