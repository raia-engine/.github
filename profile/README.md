# RaiaEngine organisation repositories

RaiaEngineの各機能は共有ライブラリに分割して開発されています。このOrganisationには、それらのプロジェクトをリポジトリに分けて管理しています。

## 

## リポジトリの構成

### ドキュメント関係

- raia-document: RaiaEngineのドキュメントを管理するリポジトリです。ドキュメントはVitePress用にMarkdown形式で書かれています。
- raia-engine.github.io: raia-documentから生成された静的サイトを公開するためのリポジトリです。(https://raia-engine.github.io)

- 実行ファイル
  - raia-core: `config.json`で指定されている共有ライブラリのinit関数を実行します。デフォルトでは組み込みスクリプトを実行するために使用しています。
  - raia-alert: コマンドライン引数で受け取った文字列をOS標準の警告ダイアログで表示します。ライブラリやスクリプトのエラーを視覚的に表示したいときに使います。
- 組み込みスクリプト用の共有ライブラリ
  - raia-v8: Googleが開発しているJavaScriptエンジンであるV8を、RaiaEngineで使えるようにするためのライブラリです。
  - raia-duktape: Cで書かれたES5.0/5.1に準拠したJavaScriptエンジンであるDuktapeを、RaiaEngineで使えるようにするためのライブラリです。
  - raia-lua: LuaをRaiaEngineで使えるようにするためのライブラリです。
  - raia-mruby: 組み込み向けの軽量Rubyであるmrubyを、RaiaEngineで使えるようにするためのライブラリです。
- サードパーティ製ライブラリをバインディングするための共有ライブラリ
  - raia-glfw: GLFW3をRaiaEngine用にバインディングしたライブラリです。
  - raia-gles: GLES3をRaiaEngine用にバインディングしたライブラリです。Googleが開発しているANGLEがベースになっています。上記と組み合わせて使います。
  - raia-imgui: ImGuiをRaiaEngine用にバインディングしたライブラリです。上記の2つと組み合わせて使います。
- APIを提供する共有ライブラリ
  - raia-draw: 原始的なピクセル操作のAPIを提供するライブラリです
  - raia-image: 画像データの読み書きのAPIを提供するライブラリです。
  - raia-font: フォントの読み込みと描画のためのライブラリです。
  - raia-file: 
- 予約
  - raia: 将来的にRaiaEngineを単に'Raia'と呼ぶようになったときのために確保しています。
  - raia-sound: サウンド関係のためのライブラリです。OpenALの使用を検討しています。
  - raia-example: RaiaEngineのサンプルを置くためのリポジトリです。
  - raia-sdk: RaiaEngineのライブラリを作るための開発キットを置くためのリポジトリです。
- 廃止予定
  - raia-gui: スクリプト側で必要な処理が書けるようになったため。
  - raia-app: スクリプト側で必要な処理が書けるようになったため。


|リポジトリ名||概要|

|raia-template||
