第30回GIS学会 ワークショップFOSS4Gを使って3D空間データを扱ってみよう！！
===

* [ワークショップサイト](https://sites.google.com/site/foss4gsig/お知らせ/第30回gis学会-ワークショップfoss4gを使って3d空間データを扱ってみよう)

開催趣旨
---

開催趣旨
　近年、国土交通省による日本全国の3D都市モデルの整備・オープンデータ化プロジェクトである「PLATEAU」や、静岡県によるバーチャル静岡のLiDAR点群データなど、多くの3次元空間情報がオープンデータとして公開されています。今後、これらのデータを活用した研究が進展することが期待されます。本ワークショップでは、FOSS4Gを用いたこれらのデータの表示、処理の方法について利用者間での情報共有をすることで、今後の活用につなげることを目標とします。

開催概要
---
* 開催日時：10月31日（日）8:30～12:00
* 開催形式：Zoomによるリモートワークショップ

ワークショップ概要
---

### ワークショップ３：Pythonで点群データを表示しよう

#### ワークショップ講師：
* 講師名：小俣 博司 (Hiroshi Omata) @homata
* プロフィール:
  * Geo + Python  JP コミュニティ
  * CIVIC TECH JAPAN/オープン川崎 

#### ワークショップの概要： 
* 点群データとは?
* ツールを使って点群データを間引き
* 点群データを表示してみる

#### 使うソフトとデータ：
##### ソフトウェア
* Google Colaboratory（略称: Colab）
* CloudCompare
* MeshLab
* Anaconda (Python and Spyder IDE)

##### 事前準備
* Google Colaboratoryが動作する環境
    * Googleアカウントにログインして、下記のファイルが動作するようにしてください
      * [Colaboratory へようこそ](https://colab.research.google.com/notebooks/welcome.ipynb?hl=ja)
* [CloudCompare](http://www.cloudcompare.org/)
* [MeshLab](http://www.meshlab.net/)
* Anaconda (Python and Spyder IDE)
    * [Anaconda のインストール](https://www.python.jp/install/anaconda/)

#### 使用データ 

##### 点群データ
* [「VIRTUAL SHIZUOKA」富士山南東部・伊豆東部エリアのデータ公開](http://www2.pref.shizuoka.jp/all/kisha20.nsf/c3db48f94231df2e4925714700049a4e/02c1ee8264a1b658492585420007c620)
* [G空間情報センター 富士山南東部・伊豆東部　点群データ](https://www.geospatial.jp/ckan/dataset/shizuoka-2019-pointcloud)

##### ワークショップの説明で使用する点群データ
* [河津七滝ループ橋：[08OF4060]（ファイルサイズ大きいです）](https://gic-shizuoka.s3-ap-northeast-1.amazonaws.com/2020/LP/00/08OF4060.zip)　
* [韮山反射炉：[08NF5045]（ファイルサイズ大きいです）](https://gic-shizuoka.s3-ap-northeast-1.amazonaws.com/2020/LP/00/08NF5045.zip) 

#### 対象者、想定（要求）レベル：
* 点群データを触ったことが無い方
* Python初心者