# SvelteKit TypeScript プロジェクト

TypeScriptで構築されたSvelteKitプロジェクトです。Cloudflare Pagesでのデプロイに対応しています。

## 開発環境

依存関係をインストールし、開発サーバーを起動します：

```bash
yarn install
yarn dev
```

## ビルド

本番用のアプリケーションをビルドします：

```bash
yarn build
```

本番ビルドをプレビューします：

```bash
yarn preview
```

## デプロイ

このプロジェクトは `@sveltejs/adapter-cloudflare` を使用してCloudflare Pagesへのデプロイに対応しています。

### 前提条件

- Cloudflareアカウント
- Wrangler CLI（開発依存関係として含まれています）

### 設定ファイル

- `wrangler.toml` - Cloudflare Workers設定
- `svelte.config.js` - SvelteKit設定（Cloudflareアダプター使用）

### GitHub Actions デプロイ

GitHubリポジトリをCloudflare Pagesと連携させることで、プッシュ時の自動デプロイが可能です。
