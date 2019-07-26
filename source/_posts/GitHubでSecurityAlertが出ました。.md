---
title: GitHubでSecurityAlertが出ました。
date: 2019-07-26 13:11:35
tags: GitHub
---
## GitHubのSecurityAlertに対応しました。
npm-check-updatesが便利でした。
```console
npm install -g npm-check-updates
ncu
ncu -u
npm install
```
1. ncu コマンドで更新があるか確認をする
2. すべて更新するならば、ncu -u で package.json を書き換え
3. npm install で更新

## 問題のあるモジュールの確認
```console
npm ls "問題のあるとされるモジュール名"
npm ls | grep "問題のあるモジュール名"
```
使用しているモジュールが依存しているモジュール、など直接使用していないモジュールの場合にこんなコマンドで更新されたのか確認してみました。

## yarn
hexo は npm でなく、 yarn を使っているようで yarn を使用したアップデートが必要でした。
