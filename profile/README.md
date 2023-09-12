# RaiaEngine organisation repositories

RaiaEngineの各機能は共有ライブラリに分割して開発されています。このOrganisationには、それらのプロジェクトをリポジトリに分けて管理しています。

## ドキュメント

（準備中）RaiaEngineに関する文書は https://raia-engine.github.io に置いています。

## リポジトリの構成

- 実行ファイル
  - [raia-core](https://github.com/raia-engine/raia-core): `config.json`で指定されている共有ライブラリのinit関数を実行します。デフォルトでは組み込みスクリプトを実行するために使用しています。
  - [raia-alert](https://github.com/raia-engine/raia-alert): コマンドライン引数で受け取った文字列をOS標準の警告ダイアログで表示します。ライブラリやスクリプトのエラーを視覚的に表示したいときに使います。
- 組み込みスクリプト用の共有ライブラリ
  - [raia-v8](https://github.com/raia-engine/raia-v8): Googleが開発しているJavaScriptエンジンであるV8を、RaiaEngineで使えるようにするためのライブラリです。
  - [raia-duktape](https://github.com/raia-engine/raia-duktape): Cで書かれたES5.0/5.1に準拠したJavaScriptエンジンであるDuktapeを、RaiaEngineで使えるようにするためのライブラリです。
  - [raia-lua](https://github.com/raia-engine/raia-lua): LuaをRaiaEngineで使えるようにするためのライブラリです。
  - [raia-mruby](https://github.com/raia-engine/raia-mruby): 組み込み向けの軽量Rubyであるmrubyを、RaiaEngineで使えるようにするためのライブラリです。
- サードパーティ製ライブラリをバインディングするための共有ライブラリ
  - [raia-glfw](https://github.com/raia-engine/raia-glfw): GLFW3をRaiaEngine用にバインディングしたライブラリです。
  - [raia-gles](https://github.com/raia-engine/raia-gles): GLES3をRaiaEngine用にバインディングしたライブラリです。Googleが開発しているANGLEがベースになっています。上記と組み合わせて使います。
  - [raia-imgui](https://github.com/raia-engine/raia-imgui): ImGuiをRaiaEngine用にバインディングしたライブラリです。上記の2つと組み合わせて使います。
- APIを提供する共有ライブラリ
  - [raia-draw](https://github.com/raia-engine/raia-draw): 原始的なピクセル操作のAPIを提供するライブラリです
  - [raia-image](https://github.com/raia-engine/raia-image): 画像データの読み書きのAPIを提供するライブラリです。
  - [raia-font](https://github.com/raia-engine/raia-font): フォントの読み込みと描画のためのライブラリです。
  - [raia-file](https://github.com/raia-engine/raia-file): ファイルの読み書きのAPIを提供するライブラリです。
- ドキュメント関係
  - [raia-document](https://github.com/raia-engine/raia-document): RaiaEngineのドキュメントを管理するリポジトリです。ドキュメントはVitePress用にMarkdown形式で書かれています。
  - [raia-engine.github.io](https://github.com/raia-engine/raia-engine.github.io): raia-documentから生成された静的サイトを公開するためのリポジトリです。(https://raia-engine.github.io)
- 予約
  - [raia](https://github.com/raia-engine/raia): 将来的にRaiaEngineを単に'Raia'と呼ぶようになったときのために確保しています。
  - [raia-sound](https://github.com/raia-engine/raia-sound): サウンド関係のためのライブラリです。OpenALの使用を検討しています。
  - [raia-example](https://github.com/raia-engine/raia-example): RaiaEngineのサンプルを置くためのリポジトリです。
  - [raia-sdk](https://github.com/raia-engine/raia-sdk): RaiaEngineのライブラリを作るための開発キットを置くためのリポジトリです。
- 廃止予定
  - [raia-gui](https://github.com/raia-engine/raia-gui): スクリプト側で必要な処理が書けるようになったため。
  - [raia-app](https://github.com/raia-engine/raia-gui): スクリプト側で必要な処理が書けるようになったため。
