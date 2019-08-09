---
title: postgresメモ
date: 2019-07-18 04:57:10
tags: PostgreSQL
---

## データベースログイン
デフォルトのユーザ postgres でログインする。
exitでログアウトできる。
```console
sudo su - postgres
```

## データベース作り直し
データベースを削除して、データベースを作成する。
```console
psql database データベース名; create database データベース名;
```

## データベースに保存できたか確認する
```console
sudo su - postgres
psql データベース名
select * from テーブル名;
```
psql データベース名 で接続する。\qで抜ける。

## データベース一覧
```console
sudo su - postgres
psql -l
```
psqlのプロンプトではバックスラッシュl(エル)
