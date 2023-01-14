# 作業ログ
## Laravelインストール
```bash
curl -s https://laravel.build/breeze-react-app | bash
cd breeze-react-app
sail up -d
```

## vscode devcontainerの追加
laravel.testを追加

## リモートコンテナでの作業

### DBマイグレーション
```
php artisan migrate
```

### breezeインストール
```
composer require laravel/breeze --dev
php artisan breeze:install react --ssr
php artisan migrate
npm install
npm run build
```

### 接続
http://localhost