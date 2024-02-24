# hugo-theme-maku

まく専用 Hugo テーマ（Hugo module）です。

自分用にカスタマイズされすぎているので汎用性がありません。使わないでください。参考にするだけならOK (^-^)


テーマの導入方法
----

### config.toml に Hugo module として追加

```toml
[params]
  facebookAppId = "1234567890123456"
  Author = "名前"
  AmazonId = "xxxx00-22"
  CustomSearchId = "partner-pub-1234567890123456:1234567890"

...
[module]
[[module.imports]]
  path = "github.com/maku77/hugo-module-maku-common"
[[module.imports]]
  path = "github.com/maku77/hugo-theme-maku"
```


Hugo module のアップデート方法
----

```console
$ go mod tidy  # これを入れておくと go.sum のエントリーが最新だけになっていい感じ
$ hugo mod get -u github.com/maku77/hugo-module-maku-common
$ hugo mod get -u github.com/maku77/hugo-theme-maku
```
