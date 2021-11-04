---
title: "Comet.mlが便利だったので記事にした" # 記事のタイトル
emoji: "🤖" # アイキャッチとして使われる絵文字（1文字だけ）
type: "tech" # tech: 技術記事 / idea: アイデア記事
topics: ["python","ai", "ml"] # タグ。["markdown", "rust", "aws"]のように指定する
published: true # 公開設定（falseにすると下書き）
---
# Comet.mlとは
実験管理ツールです。クラウドに実験結果を保存しておけます。イメージとしてはtensorboardがオンラインにあるような感じです。  

# まずはcometに登録する
GitHubアカウントで簡単に登録できます。  
https://www.comet.ml  

そして、アカウントの画像にあるメニューから「Quickstart guide」をクリックすると、認証するためのソースコードが表示できます。  

![](https://storage.googleapis.com/zenn-user-upload/2cf6869f314d558f7e01df4d.jpg)

あとはcometにある[サンプルコード](https://www.comet.ml/docs/python-sdk/pytorch/)を実行して、以下のようなURLをクリックすると別タブでサイトが開かれてログをリアルタイムで観察できます。   

`https://www.comet.ml/oshita-n/general/aaaaaaaaaaaaaaaaaa`

![](https://storage.googleapis.com/zenn-user-upload/4db039b978256ace322d8930.jpg)