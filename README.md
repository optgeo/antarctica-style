# atrantic-style


[FOSS4G 2021 Japan Online](https://www.osgeo.jp/events/foss4g-2021/foss4g-2021-japan-online) ハンズオン用のサンプルレポジトリです。


## ユーザーがカスタマイズする際の手順

* [Use this template](https://github.com/naogify/basic/generate) ボタンでこのリポジトリをコピー。
* GitHubPages を設定。
* `style.yml` を編集。
* しばらくすると `gh-pages` ブランチに `style.json` がコミットされます。
* GitHubPages の URL にアクセスすると修正した地図が表示されます。

例：https://naogify.github.io/atrantic-style

## 色のカスタマイズ

地図の色を変更するには、[layers](./layers) にあるファイル内のカラーコードを変更して下さい。

例えば [background.yml](./layers/background.yml) は以下の様になっています。海の色は `rgb(161, 229, 252)` なので `rgb(255, 0, 0)` に変更すると赤に変更できます。

```
id: background
type: background
paint: 
  background-color: rgb(161, 229, 252)
```
