---
title: hexoについて
date: 2019-06-18 02:49:46
tags: hexo
---

# なぜ、Hexoにしたのか
Node.jsで作られているから。

## インストールからローカル環境での確認までしたこと
公式サイトより以下
```console
$ npm install hexo-cli -g
$ hexo init blog
$ cd blog
$ npm install
```
vagrantにubuntuのため、開けているポートを指定して
```console
$ hexo server -p 8000
```

## GithubPagesで公開するまでにしたこと
ユーザーページの作成はすでにしていました。
\_config.ymlにdeployについて記入。
```yml
deploy:
  type: git
  repo: ユーザーページのリポジトリ
  branch: master
```
GitHubへデプロイするためにプラグインをインストール
```console
$ npm install hexo-deploy-git --save
```
以下のコマンドで、publicフォルダ内にサイトを生成し、それをデプロイしてくれるようです。
```console
$ hexo deploy -g
```

## テーマについて
テーマは採用せずに、気になったところをいじって勉強しようと思います。


