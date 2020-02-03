## 国勢調査等の政府統計データを用いたデータ分析と視覚化
今回はデータが揃った約600の市区町村を分類した。結果としては、大都市、ベッドタウン、過疎都市、等の粗い分類結果が得られた。以下は関東地域の結果。<br>

![demo](https://github.com/Jun-Tam/JapaneseCensusAnalysis/raw/master/figure/関東.png)

Class1: 持ち家ありの家族世帯<br>
Class2: 若い夫婦世帯が住む郊外<br>
Class3: 平均都市<br>
Class4: 大都会<br>
Class5: ベッドタウン<br>
Class6: 過疎化地域<br>
N/A: 田舎(データ不足のため、分析対象外)<br>


### ワークフロー
Part 1: 食材の買い出し。<br>
e-Statsからデータの取得。(参考 https://note.nkmk.me/python-e-stat-api-download/)<br>

Part 2: 下ごしらえ。<br>
使えそうな特徴量の抽出。<br>

Part 3: 調理。<br>
データの標準化。クラスタリング。主成分分析。<br>

Part 4: 盛り付け。<br>
GeopandasとPlotly Expressによる、分析結果のインタラクティブマップ作成。<br>

次回はもう少し都市部に対象を絞り、大都市のより詳細な分類を試みたい。
