# Git使い方（入門）
## 導入
[ここ](https://git-scm.com/)からDLしてインストール
## 初期設定
カレントディレクトリをGit管理の配下に置く
```git init```
インストール時の初期設定
git config user.email メールアドレス
git config user.name ユーザ名
各種設定の確認
git config --list
## add~pushの流れ
カレントディレクトリのステータスを表示する
git status
変更ファイルを管理対象に含める
git add ファイル名
addした変更点をコミットする（viなどが立ち上がる）
git commit
ワンラインでコミットする
git commit -m "ここにコメント"
リモートリポジトリに反映させる
git push origin master
git push
## リモートリポジトリを設定する（GitHub）
リモートリポジトリをpush/pullに設定する
git remote add リポジトリ名 https://github.com/ユーザ名/リポジトリ名.git/
git push --set-upstream リポジトリ名 master
## ブランチを切る
ブランチを確認する
git branch
新規ブランチを作成する
git branch ブランチ名
ブランチを移動する
git checkout ブランチ名
作成と移動をまとめてやる
git checkout -b ブランチ名
