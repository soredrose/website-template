# JavaScript
JavaScriptはGulpで連結と圧縮の処理だけをしています。

## ディレクトリ構成
JavaScriptは3つ大きくわけられます。

1. jquery
2. lib
3. namespace

JQueryは`htdocs/assets/js/`にそのまま出力されます。  
linはサイト全体で使われるライブラリやプラグインを保存します。  
namespaceはECSSの考えをベースに使われる場所や状況ごとにディレクトリをわけて、さらにModuleごとにファイルをわけます。

```
js/
├── lib/
│   ├── lodash.custom.min.js
│   ├── picturefill.min.js
│   ├── jquery.matchHeight-min.js
│   ├── focus-visible.js
│   └── smooth-scroll.min.js
├── namespace/
│   ├── js/
│   └── data/
├── jquery.min.js
└── namespace/
```

ファイルはすべて、`htdocs/assets/js/`に出力されます。
