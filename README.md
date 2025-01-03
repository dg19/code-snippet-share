# Code Snippet Share

シンプルなコードスニペット共有サービス。即座にシンタックスハイライトされ、URLで簡単に共有できます。

## 特徴

- 🚀 シンプルなUI
- ✨ リアルタイムシンタックスハイライト
- 🔗 短縮URL生成
- ⏱️ 30日後に自動削除
- 📝 50,000文字まで対応
- 🎨 主要プログラミング言語対応

## 必要要件

- Node.js (v14以上)
- MongoDB (v4.4以上)
- npm または yarn

## セットアップ手順

 1. リポジトリのクローン:
```bash
git clone https://github.com/yourusername/code-snippet-share.git
cd code-snippet-share
```
 2. サーバーのセットアップ:
```bash
cd server
npm install
cp .env.example .env  # 環境変数の設定
npm run dev
```
 3. クライアントのセットアップ:
```bash
cd client
npm install
npm start
```
 4. ブラウザで開く:
```bash
http://localhost:3000
```

## 環境変数の設定

サーバーの .env ファイルを作成し、以下の設定を行ってください：
```bash
PORT=3001
MONGODB_URI=mongodb://localhost:27017/code-snippet-share
NODE_ENV=development
```

## 開発用コマンド

### サーバー

 - 開発モード起動: `npm run dev`
 - ビルド: `npm run build`
 - 本番モード起動: `npm start` 
 - リント: `npm run lint`

### クライアント

 - 開発モード起動: `npm start`
 - ビルド: `npm run build`
 - テスト: `npm test`

## デプロイ

### サーバー

 1. ビルドの実行:
```bash
cd server
npm run build
```
 2. 本番環境での起動:
```bash
NODE_ENV=production npm start
```

## クライアント

 1. 本番用ビルドの作成:
```bash
NODE_ENV=production npm start
```
 2. build ディレクトリの内容をウェブサーバーにデプロイ

## セキュリティ対策

 - クライアント側での文字数制限
 - サーバー側でのバリデーション
 - MongoDBのインデックス設定による自動削除
 - CORSの適切な設定

## トラブルシューティング

 1. MongoDBの接続エラー:
	・MongoDBが起動していることを確認
	・正しいURIを設定していることを確認
 2. ポートの競合:
	・.envファイルで別のポートを設定
 3. ビルドエラー:
	・node_modulesを削除して再インストール
	・Node.jsバージョンの確認

## 貢献

 1. Forkする
 2. フィーチャーブランチを作成 (git checkout -b feature/amazing-feature)
 3. 変更をコミット (git commit -m 'Add amazing feature')
 4. ブランチをPush (git push origin feature/amazing-feature)
 5. Pull Requestを作成

## ライセンス

MIT License

## 作者
DG19
