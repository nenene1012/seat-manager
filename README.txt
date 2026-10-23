座席利用時間管理 PWA

ファイル構成
- index.html              本体
- manifest.webmanifest    PWA設定
- sw.js                   オフラインキャッシュ
- icon-192.png            アプリアイコン
- icon-512.png            アプリアイコン

Vercelでの公開
1. このフォルダの中身をGitHubリポジトリへアップロード
2. Vercelで Add New > Project
3. GitHubのリポジトリをImport
4. Framework PresetはOther
5. Build Commandは空欄
6. Output Directoryも空欄
7. Deploy

このアプリは静的HTMLなので npm build は不要です。
座席データはブラウザのlocalStorageに保存されます。
そのため、現状では端末間で座席状態は同期されません。
