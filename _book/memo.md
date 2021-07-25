Gitbook
----
* [Pythonではじめる地理空間情報](https://homata.github.io/geopython-book/)
* [GeoDjangoではじめる地理空間情報](https://github.com/homata/geodjango-book)
    - [https://homata.gitbook.io/geodjango/)

#### Init
* [GitBookでWebサイトを作ってGitHub Pagesで公開する方法](https://r-ngtm.hatenablog.com/entry/2020/06/18/193235)
* [GitBookによるドキュメント作成](https://qiita.com/mebiusbox2/items/938af4b0d0bf7a4d3e33)
    - https://zenn.dev/mebiusbox/articles/703e934c78fa20

Init
```
$ npm install -g gitbook-cli
$ npm init
$ gitbook init
```

test server
```
$ gitbook serve
http://localhost:4000
```

build for github pages
```
$ gitbook build . docs
```

#### Install Error

* [Gitbook-cli install error TypeError: cb.apply is not a function inside graceful-fs](https://stackoverflow.com/questions/64211386/gitbook-cli-install-error-typeerror-cb-apply-is-not-a-function-inside-graceful)
* [Gitbookの使用中に「cb.applyは関数ではありません」エラーを修正する方法](https://tech-wiki.online/jp/cb-apply-not-a-function.html)

エラー
```
$ gitbook init
Installing GitBook 3.2.3
C:\Users\homata\AppData\Roaming\npm\node_modules\gitbook-cli\node_modules\npm\node_modules\graceful-fs\polyfills.js:287
      if (cb) cb.apply(this, arguments)
                 ^

TypeError: cb.apply is not a function
    at C:\Users\homata\AppData\Roaming\npm\node_modules\gitbook-cli\node_modules\npm\node_modules\graceful-fs\polyfills.js:287:18
    at FSReqCallback.oncomplete (fs.js:169:5)
```
インストール先
```
$ npm bin -g
$ cd /usr/local/lib/node_modules/gitbook-cli/node_modules/npm/node_modules/
```
最新版にしてみる
```
$ npm install graceful-fs@latest --save
```
パッチをあてる
```
$ vi /usr/local/lib/node_modules/gitbook-cli/node_modules/npm/node_modules/graceful-fs/polyfills.js
62: // fs.stat = statFix(fs.stat)
63: // fs.fstat = statFix(fs.fstat)
64: // fs.lstat = statFix(fs.lstat)
```


Python 学習
----
* [Colaboratory とは](https://colab.research.google.com/notebooks/intro.ipynb)

* [Python-izm](https://www.python-izm.com/)
* [PythonエンジニアによるPython3学習サイト](https://www.python.ambitious-engineer.com/)
* [Python Boot Camp](https://www.pycon.jp/support/bootcamp.html)
* [ゼロからのPython入門講座](https://www.python.jp/train/index.html)

* [Binder](https://mybinder.org/)
* [GeoDjangoではじめる地理空間情報](https://homata.gitbook.io/geodjango/)
* [PyDeck](https://pydeck.gl/)
* [CheckiO](https://checkio.org/)
* [Google ColabでYOLOv5を使って物体検出してみた](https://qiita.com/shoku-pan/items/31bf3c975b73db153121)

* [無料で読める、東大／京大の「Python教科書」電子書籍](https://www.atmarkit.co.jp/ait/articles/2105/26/news025.html)
* [東京大学のデータサイエンティスト育成講座](https://www.amazon.co.jp/dp/B07PD237GQ/)


* [Python 公式サイト](https://www.python.org/)
    * [Python 3.9.4 ドキュメント](https://docs.python.org/ja/3/)
* [Python.jp プログラミング言語 Python情報サイト](https://www.python.jp/index.html)


* [GIS実習オープン教材](https://gis-oer.github.io/gitbook/book/)
    - https://github.com/gis-oer/gis-oer


*【PythonでGIS】GeoPandasまとめ
    https://qiita.com/c60evaporator/items/ac6a6d66a20520f129e6