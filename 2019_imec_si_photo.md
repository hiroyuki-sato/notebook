
## 福田昭のデバイス通信: imecが語る最新のシリコンフォトニクス技術

* [(1) 光ファイバー通信の基礎知識](https://eetimes.jp/ee/articles/1804/03/news032.html)
* [(2) 電気通信と光通信の境界](https://eetimes.jp/ee/articles/1804/10/news025.html)
* [(3) シリコンフォトニクスとは何か](https://eetimes.jp/ee/articles/1804/18/news031.html)
* [(4) シリコンフォトニクスの技術開発ロードマップ](https://eetimes.jp/ee/articles/1804/24/news032.html)
* [(5) 光送受信モジュールの技術開発ロードマップ](https://eetimes.jp/ee/articles/1805/07/news019.html)
* [(6) imecが研究中のシリコンフォトニクス・プラットフォーム ](https://eetimes.jp/ee/articles/1805/11/news032.html)
* [(7) シリコン光導波路と基本的な光波長フィルター](https://eetimes.jp/ee/articles/1805/23/news014.html)
* [(8) WDM伝送を支える光波長フィルターの特性とその制御 ](https://eetimes.jp/ee/articles/1805/29/news024.html)
* [(9) シリコン光変調器の基礎](https://eetimes.jp/ee/articles/1806/06/news031.html)
* [(10) シリコンフォトニクスで使われる主な光変調器](https://eetimes.jp/ee/articles/1806/15/news018.html)
* [(11) シリコン中のキャリア密度の増減によって光の位相を変調する](https://eetimes.jp/ee/articles/1806/25/news031.html)
* [(12) 光変調器の試作例（マッハツェンダ変調器とリング変調器）](https://eetimes.jp/ee/articles/1807/03/news016.html)
* [(13) 光変調器の試作例（電界吸収（EA）変調器）とまとめ（前編）](https://eetimes.jp/ee/articles/1807/10/news014.html)
* [(14) 光変調器の試作例（電界吸収（EA）変調器）とまとめ（後編）](https://eetimes.jp/ee/articles/1807/12/news031.html)
* [(15) シリコンフォトニクスの光検出器](https://eetimes.jp/ee/articles/1807/25/news015.html)
* [(16) 100Gbpsを超える光ファイバー高速伝送へのアプローチ ](https://eetimes.jp/ee/articles/1807/30/news026.html)
* [(17) 光ファイバーとシリコン光導波路を結合する技術](https://eetimes.jp/ee/articles/1808/07/news022.html)
* [(18) 半導体レーザーとシリコン光導波路を接続する技術（前編）](https://eetimes.jp/ee/articles/1808/16/news019.html)
* [(19) 半導体レーザーとシリコン光導波路を接続する技術（後編）](https://eetimes.jp/ee/articles/1808/20/news029.html)
* [(20) 光送受信器の構造と性能向上手法 ](https://eetimes.jp/ee/articles/1808/27/news041.html)
* [(21) 超高速光送受信モジュールの構成例](https://eetimes.jp/ee/articles/1809/04/news017.html)
* [(22) 896Gbpsの伝送帯域を実現する超高速光送受信モジュール(前編)](https://eetimes.jp/ee/articles/1809/11/news017.html)
* [(23) 896Gbpsの伝送帯域を実現する超高速光送受信モジュール(後編)](https://eetimes.jp/ee/articles/1809/14/news037.html)
* [(24) 光変調器を駆動する高速CMOS回路の試作事例](https://eetimes.jp/ee/articles/1809/26/news033.html)
* [(25) 光送受信システムのリンクバジェット計算事例](https://eetimes.jp/ee/articles/1810/04/news036.html)
* [(26) 化合物レーザーをシリコンにモノリシック集積する試み（前編）](https://eetimes.jp/ee/articles/1810/12/news035.html)
* [(27) 化合物レーザーをシリコンにモノリシック集積する試み（後編）](https://eetimes.jp/ee/articles/1810/16/news045.html)



### 第一回

* 分類
  * SONET/SDH
    * SR(Short Reach): ~2KM
    * IR(Intermediate Reach): ~ 40Km
    * LR(Long Reach) ~ 80Km
  * イーサネット(10Gbps)
    * SR(Short Range): ~ 300m
    * LR(Long Range): ~ 10Km
    * ER(Extended Range): ~ 40Km
    * ZR: ~ 80Km

### 第二回

| 種類     | 速度   | 距離   |
|----------|--------|--------|
| 電気通信 | 低速   | 短距離 |
| 光通信   | 高速   | 長距離 |

「100Gbps×1m」

* 距離: 100m = 境界1m
* 距離: 1cm = 10Tbps

| 転送種類             | 距離     | 速度              | 配線         |
|----------------------|----------|-------------------|--------------|
| 半導体内部転送       | 5cm      | 100Gbps -> 1Tbps  | 電気(銅配線) |
| ボード内部           | 50cm     | 10Gbps～100Gbpsで | 電気(銅配線) |
| ボード間の伝送       | 50cm～3m | 50Gbps ~          | 銅線・光混在 |
| データセンター内通信 | 500m ~   | ~ 200Gbps         | 光配線       |
| データセンター間     | 10km ~   | 100Gbps～200Gbps  | 光配線       |

光集積化（フォトニクスインテグレーション）-> インジウムリン（InP）を使った集積化技術

* InPを使う光集積回路の弱点
  * その1: 材料コストと製造コストが高い
  * その2: シリコンIC（CMOSデバイス）との一体化が困難

### [SOI (シリコンオンインシュレーター) の世界市場 ～2023年](https://www.gii.co.jp/report/mama134075-silicon-on-insulator.html)

第7章 SOI市場：ウェハーの種類別

* RF-SOI
* PD-SOI (部分欠乏型SOI)
* FD-SOI (完全欠乏型SOI)
* パワーSOI
* 最新式SOI
  * フォトニクスSOI
  * イメージャーSOI

## メモ

* 2018年11月現在 32nm以下でシリフォトするのは難しいらしい。[参考](https://twitter.com/ogawa_tter/status/1117748980820013056)
