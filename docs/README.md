# [docsify](https://docsify.js.org) とは

![docsify logo](https://docsify.js.org/_media/icon.svg "docsify logo")

魔法の文書サイトジェネレーター

- シンプルで軽量 :dancer:
- 静的にビルドされた html ファイルがない :ok_woman:
- 複数のテーマ :dancers:

# [Quick start](https://docsify.js.org/#/quickstart)

オフィシャルでは `docsify-cli` をグローバルにインストールすることをお勧めしている

```sh
npm i docsify-cli -g
```

## [初期化](https://docsify.js.org/#/quickstart?id=initialize)

ディレクトリを指定して初期化する

`./docs` サブディレクトリにドキュメントを書きたい場合は以下の様に指定する

```sh
docsify init ./docs
```

## [コンテンツを書く](https://docsify.js.org/#/quickstart?id=writing-content)

`init` が完了すると、`./docs` ディレクトリにファイルができる

- `index.html` アプリケーションのエントリーポイントとなるファイル
- `README.md` ドキュメントのホームページとなるファイル
- `.nojekyll` GitHub Pages でホスティングするときに [jekyll](http://jekyllrb-ja.github.io/) として処理されないようにするためのファイル

You can easily update the documentation in `./docs/README.md`, of course you can add [more pages](more-pages.md).

## [サイトをプレビューする](https://docsify.js.org/#/quickstart?id=preview-your-site)

ローカルサーバーを`docsify serve`で実行します。ブラウザで `http://localhost:3000` にアクセスするとサイトをプレビューすることができます。

```sh
docsify serve docs
```

?> `docsify-cli` の使用例については、[ドキュメント](https://github.com/docsifyjs/docsify-cli)を参照
