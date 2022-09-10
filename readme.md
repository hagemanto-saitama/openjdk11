## 概要
Java Silver SE11の検証用環境。

## ディレクトリ構成
```
.
|-- docker/                 # docker関係のファイルの置き場所
|   `-- docker-compose.yml
|-- memo/                   # ちょっとしたメモ類
|-- readme.md
`-- work/                   # 作業ディレクトリ
                            # コンテナ内の~/workとマウントしてある
```

## インストール方法
docker-compose.ymlがあるディレクトリで、下記コマンドを実行する。
```
docker-compose up -d
```

## 使い方
- お好みのテキストエディタを使用し、作業ディレクトリ(work/)内でjavaファイルを作成、編集
※work直下に直接ファイルを作成すると散らかるので、
　実際はwork下に沢山ディレクトリを作成し、
　その下で作業を行うことになると思う。
- コンテナ内でコンパイル&実行
※コンテナへの入り方
```
docker exec -it コンテナ名 bash
```