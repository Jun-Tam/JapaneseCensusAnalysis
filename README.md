## 国勢調査等の政府統計データを用いたデータ分析と視覚化
政府統計データを用いて以下のワークフローで市区町村のライフスタイル分類を実施した。<br>
都市圏の詳細な分類を試みるため、約1900ある全市区町村のうち、商業施設密度と人口密度でフィルターをかけ、<br>
285件のレコード数に対して分析を行った。そのため、N/Aのクラスが多くなっている。<br>
<br>
<br>
### ワークフロー
Part 1: 食材の買い出し。<br>
e-Statsからデータの取得。(参考 https://note.nkmk.me/python-e-stat-api-download/)<br>

Part 2: 下ごしらえ。<br>
使えそうな特徴量の抽出。<br>

Part 3: 調理と盛り付け。<br>
データの標準化。UMAPによる次元削減後、K-Meansによるクラスタリング。分類クラスの命名。<br>
GeopandasとPlotly Expressによる、分析結果のインタラクティブマップ作成。<br>
<br>
<br>
東京都・神奈川県・埼玉県の結果。<br>
![demo](https://github.com/Jun-Tam/JapaneseCensusAnalysis/raw/master/figure/東京埼玉神奈川.png)
<br>
