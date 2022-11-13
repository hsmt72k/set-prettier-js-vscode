# Prettierを使って VSCode の Javascript コードのフォーマットを設定する

## Prettier をインストール

``` console
yarn add prettier
```

## .prettierrc ファイルを作成

`.prettierrc`
``` json
{
  "printWidth": 120,
  "tabWidth": 2,
  "singleQuote": true,
  "trailingComma": "none",
  "semi": false
}
```

## VSCode の settings.json に追記

`settings.json`
``` json
{
    "editor.formatOnSave" : true,
    "[javascript]": {
        "editor.defaultFormatter": "esbenp.prettier-vscode"
      }
}
```
