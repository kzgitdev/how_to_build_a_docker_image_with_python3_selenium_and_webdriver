# How to build a docker image with python3 selenium and webdriver

## 開発環境
- ローカルパソコン：Windows10 Professional 64bit
- Docker Desktop

## 概要
Python3を使ったスクレイピングをするDockerコンテナを構築します。
Selenium をつかったheadlessなスクレイパーをいつでも使えるように記録した情報になります。

本番環境では、このDockerfileを使って以下のことが出来るようにする
- WEBスクレイピングでコンテンツを取得する
- 取得したデータをデータベースサーバー（MariaDB）に格納する
- WEBアプリケーション（PHP/Laravel）でデータベースから取得したデータを表示する
- データベースから取得したデータをトリミングして、PDFファイルとしてダウンロードできる

## Dockerfileを作成するときの注意点
- SeleniumとRequestsはそれぞれの長所・短所を理解して、状況にあわせて使い分ける。
- webdriver と google-chormeのバージョンは一致させて使いましょう。
- 
