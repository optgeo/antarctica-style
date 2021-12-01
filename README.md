# antarctica-style

これは [南極大陸のベクトルタイル](https://github.com/optgeo/a-1) のスタイルレポジトリです。

## ユーザーがカスタマイズする際の手順

```
git clone https://github.com/optgeo/antarctica-style
cd antarctica-style
npm install
```

開発環境を立ち上げる

```
npm start
```

http://localhost:8080/ で開発環境が立ち上がります。

### スタイルの公開

1. スタイルを修正後に、`main` ブランチに push します。

2. しばらくすると `gh-pages` ブランチに `style.json` がコミットされます。

3. GitHubPages の URL にアクセスすると修正した地図が表示されます。

例：https://naogify.github.io/antarctica-style/

## 色のカスタマイズ

地図の色を変更するには、[layers](./layers) にあるファイル内のカラーコードを変更して下さい。

例えば [background.yml](./layers/background.yml) は以下の様になっています。海の色は `rgb(161, 229, 252)` なので `rgb(255, 0, 0)` に変更すると赤に変更できます。

```
id: background
type: background
paint: 
  background-color: rgb(161, 229, 252)
```

参考
- https://github.com/optgeo/a-1 のタイルを使用しています。
