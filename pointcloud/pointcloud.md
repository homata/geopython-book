点群データとは？
===

点群（てんぐん）データは点（ポイント）の集まりであり、直交座標値（X,Y,Z）＋色情報（R,G,B） + αで構成された、座標参照系の情報がある3次元の空間情報データです。別名でポイントクラウドとも呼ばれています。

点群データは、地形や構造物を表すことが多く点の密度により膨大なサイズとなります。

点群データの作成方法は、LiDAR（Light Detection And Ranging）等のレーザーを利用して計測されたものや、複数の写真画像データから3次元モデルを計算して作成するSFM(Structure from Motion)やMVS（Multi-View Stereo）があり、データフォーマットとしてはLAS形式やテキストベース形式などのさまざまな形式があります。

## レーザー計測方式
点群データには、レーザーを利用して計測されたデータが多くあり、レーザー計測方式のいくつかを簡単に紹介します。

* 航空レーザ測深（ALB： Airborne Laser Bathymetry）
  * レーザースキャナーを搭載した航空機やヘリコプターから計測する
  * 複数のレーザーで、陸上と水部（河川や海の水深）を計測する方式
* 航空レーザ測量（LP： Laser Profiler）
  * レーザースキャナーを搭載した航空機やヘリコプターから計測する
  * 陸上を計測する方式
  * 従来から幅広く実施されている方式
* 移動計測車両（MMS：Mobile Mapping System）
  * レーザースキャナーを搭載した車両が道路を走りながら計測する
* 地上型または固定型
　* 移動しないで計測する方式で、3Dレーザースキャナー等の計測機を使用して計測する

そのほかに、水中設置型や、LiDARを搭載したUAV(Unmanned Aerial Vehicle)やiPhoneやiPadからも作成されます。

#### 参考
* [公共測量 - マニュアル・要領等のダウンロード (国土地理院)](https://psgsv2.gsi.go.jp/koukyou/download/download.html)
  * [航空レーザ測深機を用いた公共測量](https://psgsv2.gsi.go.jp/koukyou/public/alb/index.html)
    * [PowerPoint（PDF）](https://www.gsi.go.jp/common/000218811.pdf)

----------------------------------

## 3次元データのファイル形式

3次元データのファイルにはさまざまなファイル形式があります。
いくつかのファイルフォーマットを紹介します

### 点群データ系

####  LAS形式
* 航空機レーザー測量の標準フォーマット
* ASPRS(米国写真測量学会：American Society for Photogrammetry and Remote Sensing) によって作成された形式
  * [LAS 1.4 Specification Approved by ASPRS Board](https://www.asprs.org/news/press-releases/press-release-archives/las-1-4-specification-approved-by-asprs-board.html)
    * [LAS SPECIFICATION VERSION 1.4 – R13 15 July 2013](https://www.asprs.org/wp-content/uploads/2010/12/LAS_1_4_r13.pdf)
* [LAS Point Cloud Format](https://www.usna.edu/Users/oceano/pguth/md_help/html/las_format.htm)
* 投影座標系はUTMなどの投影座標系が推奨されいる。日本では、日本測地系2011や平面直角座標系で提供されている

####  LAZ形式
* LAS形式を圧縮したデータ形式
* [LASzip - free and lossless LiDAR compression](https://laszip.org)

####  PLY形式 (Polygon File Format)
* 3Dスキャナーから3次元データを格納するために設計されたデータ形式
* ASCIIとバイナリの2つのバージョンが存在
* [PLY - Polygon File Format]( http://paulbourke.net/dataformats/ply/)

#### XYZ、CSV、TXT形式
* タブ、空白、カンマなどでデータを区切られたASCIIファイル
* 1行目にヘッダーあり/なしがある
* 位置情報（X座標、Y座標、Z座標）と色情報（R、G、B）がある

### メッシュデータ系

#### STL形式 (Standard Triangulated Language)
* 3D CADソフト用のファイルフォーマットの1つ
* 対応している3Dプリンターが多い
* 色やカーブ形状などが表現できない
* ASCII形式とバイナリ形式がある
* [The STL Format - Standard Data Format for Fabbers](http://www.fabbers.com/tech/STL_Format)

#### OBJ形式
* Wavefront Technologies社によって開発されたファイル形式
* 多くの3Dモデリング、レンダリングソフトが対応
* 動かない3Dオブジェクトに適している
* [Obj Specification as used by Wavefront](http://www.martinreddy.net/gfx/3d/OBJ.spec)

#### FBX形式
* AutoDesk社が公開したファイル形式
* 3DCG(3 Dimensional Computer Graphics)のデファクトフォーマット
* 動く3Dオブジェクトに適している
* [Adaptable file format for 3D animation software](https://www.autodesk.com/products/fbx/overview)
