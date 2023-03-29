# 2020Kokusei-PMTiles

## データについて
- 本データは、[政府統計窓口（e-stat）](https://www.e-stat.go.jp/)にて公開されている、[2020年国勢調査小地域（町丁・字等別及び基本単位区）の境界データ（JGD2011）](https://www.e-stat.go.jp/gis/statmap-search?page=1&type=2&aggregateUnitForBoundary=A&toukeiCode=00200521)を[tippecanoe](https://github.com/felt/tippecanoe)で[PMTiles形式](https://github.com/protomaps/PMTiles)に変換したデータになります。
- オープンソースソフトウェアで構築

## デモサイト
- https://shi-works.github.io/2020Kokusei_PMTiles/
- サンプル画像
![image](https://user-images.githubusercontent.com/71203808/227753143-b5050ccb-3e4d-4b29-8778-5fe4ba2fc3d0.png)

## データ配布
### 町丁・字等別
- `https://pmtiles-data.s3.ap-northeast-1.amazonaws.com/r2kokusei/r2ka01-47_JGD2011.pmtiles`(414.9MB)
- `https://pmtiles-data.s3.ap-northeast-1.amazonaws.com/r2kokusei/r2ka01-47_point_JGD2011.pmtiles`(71.5MB)

### 基本単位区
- `https://pmtiles-data.s3.ap-northeast-1.amazonaws.com/r2kokusei/r2kb01-47_JGD2011.pmtiles`(1.1GB)
- `https://pmtiles-data.s3.ap-northeast-1.amazonaws.com/r2kokusei/r2kb01-47_point_JGD2011.pmtiles`(347.5MB)

## ベクトルタイル設計情報
### ■ 町丁・字等別
#### 境界データ（r2ka01-47_JGD2011.pmtiles）
- 境界データそのものを可能な限り生かしたデータです。
- tippecanoeによるデータの間引きを行っていません。

#### 図形中⼼点（r2ka01-47_point_JGD2011.pmtiles）
- 町丁・字等名称や人口等のラベルを表示できるようにするためのポイントデータです。
- tippecanoeによるデータの間引きを行っていません。

### ズームレベル範囲
- 10-14

### 属性
- 境界データの属性はそのまま生かしています。

### ■ 基本単位区
#### 境界データ（r2kb01-47_JGD2011.pmtiles）
- 境界データそのものを可能な限り生かしたデータです。
- tippecanoeによるデータの間引きを行っていません。

#### 図形中⼼点（r2kb01-47_point_JGD2011.pmtiles）
- 人口等のラベルを表示できるようにするためのポイントデータです。
- tippecanoeによるデータの間引きを行っていません。

### ズームレベル範囲
- 12-14

### 属性
- 境界データの属性はそのまま生かしています。

## 境界データの定義書（e-stat）
### 小地域（町丁・字等）（JGD2011）
- `https://www.e-stat.go.jp/gis/statmap-search/data?datatype=2&serveyId=A002005212020&downloadType=1&datum=2011`
### 小地域（基本単位区）（JGD2011）
- `https://www.e-stat.go.jp/gis/statmap-search/data?datatype=2&serveyId=B002005212020&downloadType=1&datum=2011`

## PMTiles Viewer
- PMTilesはPMTiles Viewerで閲覧することができます。
- https://protomaps.github.io/PMTiles/

## ライセンス
本データセットは[CC-BY-4.0](https://github.com/shi-works/2020Kokusei_PMTiles/blob/main/LICENSE)で提供されます。使用の際には本レポジトリへのリンクを提示してください。
