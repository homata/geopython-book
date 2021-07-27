MacOSのPythonのインストール
========

Python for Macを <https://www.python.org/downloads/mac-osx/>　から最新版の「Latest Python 3 Release - Python 3.6.5」(2018年6月4日現在)をダウンロードしてください。

    Python Releases for Mac OS X
        Latest Python 3 Release - Python 3.6.5
        Latest Python 2 Release - Python 2.7.15


OSの環境によって、macOS 64-bit/32-bit installer(for Mac OS X 10.6 and later)または、macOS 64-bit installer（for OS X 10.9 and later）を選択してダウンロードしてください。
ダウンロードされたら、pkgファイル（python-3.6.5-macosx10.6.pkg）をクリックしてインストーラーを実行してください。

インストールが正しく行われたか確認するために、 ターミナルを開いて「python3」もしくは「python」コマンドをタイプしてみてください

    $ python -V
    Python 3.6.5

<u>**注意**</u><br>
Macの場合、デフォルトでpython2がインストールされています。必ずバージョンを確認して
「python -V」が2系だった場合は、「python3」を使うようにしてください。「python3」だった場合はこれ以降は「python」を「python3」と読みかえてください

    $ python -V
    Python 2.7.14

    $ python3 -V
    Python 3.6.5

pipのバージョンも確認します。pipも、Pythonと同様に環境によりpip3となる場合があります。これも「pip」を「pip3」と読みかえてください

    $ pip3 --version
    pip 9.0.3 from xxx (python 3.6)


