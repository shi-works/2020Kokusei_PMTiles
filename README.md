# R2Kokusei-PMTiles

## データについて
- 本データは、政府統計窓口（e-stat）にて公開されている、[2020年国勢調査小地域（町丁・字等別及び基本単位区）](https://www.e-stat.go.jp/gis/statmap-search?page=1&type=2&aggregateUnitForBoundary=A&toukeiCode=00200521)を[tippecanoe](https://github.com/felt/tippecanoe)で[PMTiles形式](https://github.com/protomaps/PMTiles)に変換したデータになります。
- オープンソースソフトウェアで構築

## デモサイト
- https://shi-works.github.io/R2Kokusei_PMTiles/
- サンプル画像
![image](https://user-images.githubusercontent.com/71203808/227701862-d0b34585-7b7e-47b6-bbfc-422752494cd7.png)

## データ配布
- `https://pmtiles-data.s3.ap-northeast-1.amazonaws.com/maff-fude/fude_2022_01_47_centroid.pmtiles`(1.2GB)
- `https://pmtiles-data.s3.ap-northeast-1.amazonaws.com/maff-fude/fude_2022_01_47.pmtiles`(19.5GB)

## ベクトルタイル設計情報
### ■ 重心(fude_2022_01_47_centroid.pmtiles)
- 筆ポリゴンがある位置を小縮尺でも把握できるようにするための重心データです。
- tippecanoeによるデータの間引きを行っていません。

#### ズームレベル範囲
2-13

#### 属性
属性は全て外してあります。

### ■ 筆界(fude_2022_01_47.pmtiles)
- 筆ポリゴンそのものを可能な限り生かしたデータです。
- tippecanoeによるデータの間引きを行っていません。

#### ズームレベル範囲
12-16

#### 属性
- 筆ポリゴンの属性はそのまま生かしています（前前年筆ポリゴンID以外）。
- 結果として、次の属性がついていると認識しています。

- 属性項目名 名称
- polygon_uuid 筆ポリゴンID
- land_type 耕地の種類
- issue_year 公開年度
- edit_year 調製年度
- history 履歴
- last_polygon_uuid 前年筆ポリゴンID
- local_government_cd 地方公共団体コード
- point_lng 重心点座標（経度）
- point_lat 重心点座標（経度）
