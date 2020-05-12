# backlog Postman Collection について

プロジェクト管理のクラウドサービス [backlog](https://backlog.com/ja/) のAPIへ手軽にアクセスできるように作成した [Postman Collection](https://www.postman.com/collection/) ファイルです。

API 開発・検証のためのコラボレーションツール [Postman](https://www.postman.com/) にインポートして利用できます。

英語版と日本語版があり、好きな方をインポートして使ってください。

[Backlog API Reference](https://developer.nulab.com/ja/docs/backlog/) を元に作成しています。

# 使い方

## Collection ファイルのインポート

この Github リポジトリからJSONファイルをダウンロードして、Postmanにインポートするだけです。

![import](https://cdatajbuilds.s3-ap-northeast-1.amazonaws.com/CDataBlog/backlog/collectionimport.gif)

## 認証設定

Collection には予めAPI Keyを使った認証が実施できるようになっているので、backlog のユーザー設定画面から、API Keyを生成し、環境変数を書き換えてください。合わせて接続先のURLも調整してください。

![authentication](https://cdatajbuilds.s3-ap-northeast-1.amazonaws.com/CDataBlog/backlog/authentication.gif)

## データの取得

GET系のエンドポイントはデータを取得することができます。「プロジェクト一覧の取得」や「課題一覧の取得」はそのまま実行して試すことができます。

また、Paramsには backlog APIで利用できるすべてのクエリパラメータが登録されています。実行したいクエリを有効化して、任意のパラメータ値を設定すれば簡単にフィルターなどが実施できます。

DescriptionにはAPI Referenceから引用したパラメータの説明文も入っているので、どんな値を設定すればいいかもわかりやすいかなと思います。

![getlist](https://cdatajbuilds.s3-ap-northeast-1.amazonaws.com/CDataBlog/backlog/getlist.gif)

## データの追加・更新・削除

データの登録・更新・削除も実施できます。以下はプロジェクトの操作例です。

Bodyタブに予め登録できるパラメータの一覧が表示されているので、必要な値を入力もしくは入力しないパラメータを無効化してリクエストしてみてください。VALUE欄には予めその値の型も指定されていますし、Descriptionで必須項目かどうかも確認できます。

![cud](https://cdatajbuilds.s3-ap-northeast-1.amazonaws.com/CDataBlog/backlog/cud.gif)

## 添付ファイルの送信

ほとんどの操作は上記手順で実施できますが、例外として「添付ファイルの送信」機能があります。

これはBodyのValue欄からファイルを選択して実行します。

![sendattach](https://cdatajbuilds.s3-ap-northeast-1.amazonaws.com/CDataBlog/backlog/attach.gif)

## コードから実行

また、プログラムから実行したい場合にもPostmanは便利です。Codeスニペットの機能を使って、各プログラミング言語での簡単な実行コードを入手できます。

以下はVisual Studio から C# で backlog の APIを実行してみたものです。

![code](https://cdatajbuilds.s3-ap-northeast-1.amazonaws.com/CDataBlog/backlog/code.gif)

# その他

## 未対応トピック

- Example レスポンス：要望があれば、検討したいと思います。
- OAuth 認証の設定：API Keyを優先しました。

## 問い合わせについて

この Github の Issue もしくは各SNSアカウントまで。

## 関連記事

- [backlog API のための Postman Collection を公開してみました](https://www.cdatablog.jp/entry/backlogpostmancollection)

- [プロジェクト管理ツール backlog の API の使い方](https://www.cdatablog.jp/entry/backlogapi)

## 作者

[CData Software Japan 合同会社](https://www.cdata.com/jp/) Lead Engineer 杉本 和也

SNS Account : [Facebook](https://www.facebook.com/sugimomoto) / [Twitter](https://twitter.com/sugimomoto) / [Linkedin](https://www.linkedin.com/in/sugimotok/) / [Instagram](http://instagram.com/sugimomoto/) / [GitHub](https://github.com/sugimomoto)
