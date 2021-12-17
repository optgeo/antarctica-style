# antarctica-style

This is the style repository for [Antarctica vector tiles](https://github.com/optgeo/a-1).

## Demo

https://optgeo.github.io/antarctica-style/

## Instructions for style customization.

```
git clone https://github.com/optgeo/antarctica-style
cd antarctica-style
npm install
```

Set up the development environment

```
npm start
```

The development environment will be launched at http://localhost:8080/.


### Deploy map for preview

1. After modifying the style, push it to the `main` branch.

1. After a while, the `style.json` will be committed to the `gh-pages` branch.

1. If you access the GitHubPages URL, you will see the modified map. (You need to configure GitHubPages).

Example: https://optgeo.github.io/antarctica-style/

## Color customization

To change the color of the map, use [layers](./layers), change the color code in the file.

For example, in [background.yml](./layers/background.yml) looks like the following. The color of the ocean is `rgb(161, 229, 252)`, so changing it to `rgb(255, 0, 0)` will change ocean's color to red.

You can change it to red by changing it to `rgb(255, 0, 0)`.

```
id: background
type: background
paint: 
  background-color: rgb(161, 229, 252)
```

## Reference

- Uses tiles from https://github.com/optgeo/a-1.

[日本語訳はこちら](https://github.com/optgeo/antarctica-style/blob/main/README-JA.md)
