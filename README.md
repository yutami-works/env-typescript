# env-typescript

TypeScriptの環境構築と基礎的なコンパイルまで

## 環境構築

Node.js環境で実行する

```shell
$ node -v
# v18.17.1
```

グローバルにインストールして使う

```shell
$ npm install -g typescript
```

インストール確認

```shell
$ tsc -v
# Version 5.2.2
```

## コンパイル

tscコマンドでtsファイルに問題点がないかチェックできる

```shell
$ tsc increment.ts
# increment.ts:6:23 - error TS2345: Argument of type 'string' is not assignable to parameter of type 'number'.
```

コンパイルを通して問題点が無い場合はjsファイルが生成される

```shell
$ tsc increment2.ts
# 何も表示されずincrement2.jsが生成される
```