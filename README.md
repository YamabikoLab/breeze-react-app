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
yarn install
```

### npm run devで画面が真っ白になる現象に対応
https://laracasts.com/discuss/channels/vite/laravel-vite-err-address-invalid
```
export default defineConfig({
    server: {
        host: '0.0.0.0',
        hmr: {
            host: 'localhost'
        }
    },
    server: {
        host: '0.0.0.0',
        hmr: {
            host: 'localhost'
        }
    },
```

### npm run dev

```
yarn dev
```

### 接続
http://localhost

# 参考資料
## Laravel 9.x インストール
https://readouble.com/laravel/9.x/ja/installation.html

## Laravel 9.x スターターキット
https://readouble.com/laravel/9.x/ja/starter-kits.html

## inertia
https://inertiajs.com/

## vscode devcontainers
https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers
https://code.visualstudio.com/docs/devcontainers/containers