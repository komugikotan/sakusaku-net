# Sakusaku-Net
通信制限下でも、サクサクインターネットを閲覧できる検索エンジン型のサービスです。具体的には、インターネット上のウェブサイトの容量を、画像を軽量化することと、本文だけを抽出して表示することによって読み込みを高速化します。

[このURL](http://komugio.starfree.jp/sakusaku/)にアクセスしてください。トップページが表示されますので、通常の検索エンジンと同じように利用してください。

## インストール

このリポジトリをクローンして、任意のサーバーソフトでホストしてください。このソフトはPHP v8.0で作成されましたので、このバージョンを使うことをお勧めします。

サーバー側の要件は以下です。

・PHPがホストできること

・外部APIを叩けること

・サーバー内でファイルなどを作成したりできること

クライアント側の要件は以下です。

・webp対応のブラウザ

・スマホ(基本的にスマホ用のサイトなので、パソコンでは表示が崩れます)

### .envファイル

このリポジトリのルートフォルダに、.envファイルを作成する必要があります。

.envファイルには、Google Custom Search APIのAPI Keyと、Google カスタム検索エンジンの検索エンジンIDを書き込む必要があります。

このサイトは検索結果の取得にGoogle Custom Search JSON APIを使用している為です。

一行目はコメントアウトで、二行目にAPI Key, 三行目に検索エンジンIDが記録されています。環境変数などは使っておらず、ただ単にPHP上からテキストファイルとして読み出しているだけなので、APIKey=などの形にする必要はない為、直接書き込んでください。

## 貢献する

このリポジトリへのIssues, Pull Requestなどは大歓迎です。基本的にルールなどはありませんが、常識に従って頂ければどんどん送ってください。マージするかもしれません。
