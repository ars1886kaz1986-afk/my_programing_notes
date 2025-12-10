2025/12/2 - Node / npm ci と npm install の違い

- npm install
  ・package.json に基づき node_modules をインストール
  ・既存の node_modules は差分だけ更新
  ・新しいパッケージ追加時に package-lock.json を更新
  ・開発中に使用

- npm ci
  ・package-lock.json に厳密に従い node_modules を完全再構築
  ・既存の node_modules は削除される
  ・高速で再現性のあるインストール
  ・CI/CD や本番環境に最適
