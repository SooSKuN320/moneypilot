# MoneyPilot PWA (iPhone向け)

## GitHub Pagesで公開
1. GitHubで新しいリポジトリ（例: `moneypilot`）を作成。公開リポジトリで構いませんが、**家計のJSONデータを絶対にアップロードしないでください**。
2. このZIPを解凍し、`MoneyPilot_PWA`フォルダの**中身**（index.html、sw.js、manifest.webmanifest、iconsフォルダ）をリポジトリ直下へアップロード。
3. Settings → Pages → Build and deployment → Deploy from a branch → `main` / `(root)` → Save。
4. 数分後、Pagesに表示された `https://ユーザー名.github.io/moneypilot/` をiPhoneのSafariで開く。
5. Safariの共有ボタン → 「ホーム画面に追加」→「追加」。

## データ引き継ぎ
「設定・保存」→ JSONから復元で、以前の初期データJSONを**iPhone上でのみ**読み込んでください。残高と日付は古いので、読み込み後に最新残高を入力してください。

## 注意
- GitHub Pagesにはアプリのコードのみを公開。取引履歴、口座残高、バックアップJSONはアップロード禁止。
- 保存はiPhoneのブラウザ内（localStorage）。iPhone機種変更時には自動同期されません。定期的にJSONを書き出し、iCloud Drive等に安全に保管してください。JSONは暗号化されていません。
- 同じサイトでもSafariとホーム画面アプリでは保存領域が異なる場合があります。初回の保存・再起動テストを推奨します。
- GitHub Pagesは静的サイト配信で、銀行口座と自動連携しません。
- iPhone実機での動作確認は未実施です。
