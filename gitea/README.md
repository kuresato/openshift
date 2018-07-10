# Gitea

## ここのが使えそう 2018/7/10

* https://github.com/wkulhanek/docker-openshift-gitea/tree/master/openshift
* https://hub.docker.com/r/wkulhanek/gitea/

## ここのが使えそうだったけど古くなってきた

> https://github.com/willemvd/gitea-unprivileged-docker

初回起動時にインストール画面が表示されたら、以下のように入力する

* データベース設定
  * データベースの種類: SQlite3
  * パス: (デフォルトのまま /data/gitea/gitea.db）
* Giteaの全般設定
  * アプリケーション名: 好きな名前を
  * リポジトリのルートパス: デフォルトのまま(/data/git/repositories)
  * LFS Root Path: デフォルトのまま(空)
  * 実行ユーザ: たぶんデフォルトのgitのままで大丈夫
  * ドメイン: URL
  * SSHポート: とりあえずデフォルトの22のままで
  * HTTPポート: たぶん3000のままで大丈夫
  * アプリケーションのURL: 作られたrouteのURL
  * ログのパス: デフォルトのまま(/data/gitea/log)
* オプション設定
  * とりあえず全部デフォルト(必要に応じて管理者アカウント作成など)

