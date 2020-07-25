【開発準備編】

1 : Laravelプロジェクト作成
composer create-project --prefer-dist laravel/laravel vue-laravel-spa

2 : laravel/uiインストール
Laravelでフロントエンド開発をするためのベースを簡単に提供してくれるツール。
composer require laravel/ui

3 : laravel/ui vueインストール
laravel/uiを使うと、bootstrapやvue、reactなどさまざまなフロントエンドのベースコードを生成できます。
php artisan ui vue

4 : フロントエンドパッケージインストール
laravel/uiのvueベースをインストールした際に、必要なフロントエンドパッケージがpackage.jsonに追記されました。bootstrap、jquery、vueなどが追記されています。
npm install

5 : Vue Routerインストール
Vue Routerとは、Vue.jsでSPAを構築するためのルーティング処理を行うVue公式のツールです。
npm install --save vue-router

6 : フロントエンドビルド実行
必要なパッケージは全てインストール完了したので、最後にフロントエンドソースコードをビルドしてみます。
npm run dev

※今後jsファイルやcssファイル、vueコンポーネントを更新した際は、毎回 npm run dev でソースをビルドしないと画面に反映されないので注意してください。
※毎回ビルドを実行するのが面倒な場合はnpm run watch を実行するとウォッチモードになりビルド対象ファイルを更新、保存すると自動でビルドが実行されるようになるので便利です。
