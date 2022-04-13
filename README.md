# hugo-theme-maku

まく専用 Hugo テーマです。

自分用にカスタマイズされすぎているので汎用性がありません。使わないでください。参考にするだけならOK (^-^)


テーマの導入方法
----

### Hugo プロジェクトに Git submodule として追加

```console
$ cd <Hugoプロジェクト>
$ git submodule add -b main https://github.com/maku77/hugo-theme-maku.git themes/maku
$ git add .
$ git commit
```

### config.toml にテーマ設定

```toml
...
theme = "maku"
googleAnalytics = "UA-XXXXXXXX-X"

[markup.goldmark.renderer]
  unsafe = true

[params]
  facebookAppId = "1234567890123456"
  Author = "名前"
  AmazonId = "xxxx00-22"
  CustomSearchId = "partner-pub-1234567890123456:1234567890"
```


テーマ導入後の Hugo プロジェクトの扱い方
----

### テーマの submodule ごと clone する

```config
$ git clone --recursive https://github.com/<owner>/<repo>.git
```

### テーマの submodule を更新する

```config
$ git submodule update
```
