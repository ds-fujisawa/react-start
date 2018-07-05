# Reactスターターキット
フロントエンド開発は色々と複雑化していて環境構築や設定等が大変だと感じたのでスターターキットを作ってみました。  
Reactベースで作りましたが他ライブラリやライブラリなしでも応用は効くと思いますので、環境に合わせて適宜変更してご使用ください。

## 使い方
本リポジトリをクローン又はダウンロードし、`yarn install`を実行してお使いください。  
※`npm install`の場合、エラーが出る可能性があります

## 構成

```
react-start
├─ .storybook              // Storybook設定ファイル群
├─ flow-typed              // Flow型定義ファイル群
├─ public                  // 開発環境で出力されるディレクトリ
|  ├─ dev                  // 開発用データ群
|  |  └─ mock.json         // jsonデータ(APIモック用)
|  ├─ index.js             // 出力ソース
|  └─ index.html           // 確認用HTML
├─ src
|  ├─ test
|  |  ├─ index.test.js     // テストコード
|  |  └─ setupTest.js      // テスト設定ファイル
|  ├─ App.jsx              // ルート
|  └─ index.js             // エントリーポイント
├─ stories
|  └─ index.stories.js     // Storybookファイル
├─ .babelrc                // babel設定ファイル
├─ .eslintignore           // eslint対象外設定ファイル
├─ .eslintrc               // eslint設定ファイル
├─ .flowconfig             // flow設定ファイル
├─ package.json            // npm設定ファイル
├─ webpack.config.js       // Webpack設定ファイル
└─ yarn.lock   	           // バージョン固定ファイル
```

## コマンド一覧

|||
|:--|:--|
|build|publicディレクトリにjsファイルなどを出力します|
|lint|構文チェックを行います|
|lint-fix|構文チェックとフォーマットを行います|
|test|テストコードを実行します|
|flow|型チェックを行います|
|start|開発サーバが起動します(APIモックも同ポートで起動)|
|storybook|コンポーネントカタログサーバが起動します|
|build-storybook|コンポーネントカタログを出力します|

※上記コマンドには記載していませんが、gitコミット時にlint-fixコマンドが実行されるようになっています

## 主な使用パッケージ

|||
|:--|:--|
|[React](https://reactjs.org/)|UIライブラリ|
|[Styled-Components](https://www.styled-components.com/)|CSS in JSライブラリ(JSの中にCSSが記述できる)|
|[Storybook](https://storybook.js.org/)|コンポーネントカタログ|
|[Webpack](https://webpack.js.org/)|モジュールバンドラー|
|[Babel](https://babeljs.io/)|トランスパイラ(ES5に変換するツール)|
|[Jest](https://facebook.github.io/jest/)|ユニットテストライブラリ|
|[Enzyme](https://airbnb.io/projects/enzyme/)|テストユーティリティライブラリ|
|[ESLint](https://eslint.org/)|コード静的チェッカー|
|[Prettier](https://prettier.io/)|コード自動フォーマッター|
|[Flow](https://flow.org/)|型チェッカー|
