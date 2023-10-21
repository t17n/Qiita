---
title: Gitt超入門（初期設定）
tags:
  - Git
  - GitHub
private: false
updated_at: '2023-10-21T20:56:05+09:00'
id: 2d4bfd9ae59e0a3db800
organization_url_name: null
slide: false
ignorePublish: false
---
# この記事について
この記事は、自身の学習振返り・アウトプットを目的として作成しました。
自身と同じく未経験でエンジニア転職を目指す初学者の方にも見易い内容にしていければと思います。

今回は、Gitの初期設定についてです。


## ユーザー名設定
git configコマンドを使います。
```
<!-- git config コマンド -->
git config --[設定ファイルの種類] [設定項目] [設定する値]
```

下記のコードでは、
[設定ファイルの種類]・・・global
[設定項目]・・・user.name
[設定する値]・・・"自身のGitHubユーザー名"
です。
エラーが無ければ何も表示されません。

```
git config --global user.name "自身のGitHubユーザー名"
```


## メールアドレス設定
続けて下記を入力しメールアドレスを設定します。
こちらもエラーが無ければ何も表示されません。
```
git config --global user.email "自身のGitHubメールアドレス"
```


## ユーザー名・メールアドレス設定確認
登録されたか確認する場合は、以下を一文ずつ入力すると、ユーザー名・メールアドレスが返ってきます。
```
git config --global user.name
git config --global user.email
```
設定全般項目を表示する場合は、listオプションを使います。
```
git config --global --list
```

## デフォルトブランチ設定確認
最後にデフォルトブランチを確認します。
```
git config init.defaultBranch
```
上記を入力して`main`が表示されない場合は、デフォルトブランチを`main`に変更します。
```
<!-- デフォルトブランチを`main`に変更 -->
git config --global init.defaultBranch main
```


以上です。
今回始めてQiita投稿させて頂きました。
今後も習熟度向上の為に継続していきたいと思います。
