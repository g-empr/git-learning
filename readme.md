# Git使い方（入門）  
## 導入  
[ここ](https://git-scm.com/)からDLしてインストール  
## 初期設定  
カレントディレクトリをGit管理の配下に置く  
```
git init
```
ユーザ設定  
```
git config user.email メールアドレス  
git config user.name ユーザ名  
```
各種設定の確認  
```
git config --list
```
## add~pushの流れ  
カレントディレクトリのステータスを表示する  
```
git status
```
変更ファイルを管理対象に含める  
```
git add ファイル名
```
管理対象にした変更点をコミットする（viなどが立ち上がる）  
```
git commit
```
ワンラインでコミットする  
```
git commit -m "ここにコメント"
```
リモートリポジトリに反映させる  
```
git push origin master
git push
```
## ローカルリポジトリ最新化  
リポジトリの状態を更新する（リモートリポジトリの状態と同じにする）
```
git pull origin master
git pull
```
ローカルリポジトリをpush/pullするリモートリポジトリを設定する  
```
git remote add origin https://github.com/ユーザ名/リポジトリ名.git/
git push --set-upstream origin master
```
## ブランチ  
ブランチを確認する  
```
git branch
```
新規ブランチを作成する  
```
git branch ブランチ名
```
ブランチを移動する  
```
git checkout ブランチ名
```
作成と移動をまとめてやる  
```
git checkout -b ブランチ名
```
## その他
GitHubにあるリポジトリを持ってくる
```
git clone https://github.com/ユーザ名/リポジトリ名.git
```