---
title: 自分一人での GitHub 利用の流れ
date: 2019-07-17 01:01:20
tags: GitHub
---
# 私個人の、かつ一人でのGitHubを使った制作の流れのメモ

## プロジェクトを作成してデプロイまで
1. express --view=pug プロジェクト名
2. cd プロジェクト名
3. echo "node_modules/" >> .gitignore
4. npm install
5. GitHub でリポジトリを作る(Initializeにチェックは入れない)
6. echo "# プロジェクト名" >> README.md
7. git init
8. git add .
9. git commit -m "first commit"
10. git remote add origin git@～この辺りまではGitHubの指示通り
11. git push -u origin master
12. Heroku にて、Appを作り、GitHub連携でデプロイする

## 作業
1. git branch ブランチ名（何をするブランチかわかる名前）
2. git checkout ブランチ名
3. 作業
4. git add .
5. git commit -m "何をしたか"
6. git push origin ブランチ名
7. pull requestをする
8. 問題がなければマージ
9. デプロイ
10. git checkout master
11. git pull
12. git branch -d ブランチ名


