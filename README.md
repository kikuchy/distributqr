# DestributqR

AWS S3に置かれているオブジェクトへのURLを短縮して出力します。

頒布用にQRコードのEPSファイルを生成します。

## 動作環境

* MacOS X (クリップボードへのコピーに `pbcopy` を使用しています)
* qrencode (HomeBrewとかでインストールしておく必要があります)

## 環境変数

以下の環境変数がセットされている必要があります。

* `AWS_ACCESS_KEY_ID` ... 目的のS3バケットへのアクセス権限があるアクセスキー
* `AWS_SECRET_ACCESS_KEY` ... 同シークレット
* `GOOGLE_API_KEY` ... Google URL ShortenerのAPIを有効にしたAPIキー

## 使い方

    ./bin/distributqr bucket_name key_name
