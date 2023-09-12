# RaiaEngine organisation repositories

RaiaEngineの各機能は共有ライブラリに分割して開発されています。このOrganisationには、それらのプロジェクトをリポジトリに分けて管理しています。

## 

## リポジトリの案内

### ドキュメント関係

- raia-document: RaiaEngineのドキュメントを管理するリポジトリです。ドキュメントはVitePress用にMarkdown形式で書かれています。
- raia-engine.github.io: raia-documentから生成された静的サイトを公開するためのリポジトリです。(https://raia-engine.github.io)

### 実行ファイル

- raia-core: `config.json`で指定されている共有ライブラリのinit関数を実行します。デフォルトでは組み込みスクリプトを実行するために使用しています。
- raia-alert: コマンドライン引数で受け取った文字列をOS標準の警告ダイアログで表示します。ライブラリやスクリプトのエラーを視覚的に表示したいときに使います。

### 組み込みスクリプトのためのリポジトリ

- raia-v8
- raia-duktape

### RaiaAPIを提供する共有ライブラリのリポジトリ

raia-imgui
raia-gles
raia-draw
raia-image
raia-font
raia-glfw

### 廃止予定

raia-gui
raia-app


|リポジトリ名||概要|

|raia-template||
