* アメリカ？規格団体

  * [ANSI](https://www.ansi.org) 米国国家規格協会(American National Standards Institute)
  * [TIA](https://www.tiaonline.org) (米国の)電気通信工業会(Telecommunications Industry Association)
  * [EIA]() 電子工業会(Electronic Industries Alliance) もう古い？
    * [EIA Standards](https://en.wikipedia.org/wiki/EIA_standards)

* 国際規格団体
  * [ISO](https://www.iso.org/home.html) 国際標準化機構(International Organization for Standardization)
  * [IEC](https://www.iec.ch) 国際電気標準会議(International Electrotechnical Commission)
  * [ISO/IEC JTC 1](https://ja.wikipedia.org/wiki/ISO/IEC_JTC_1) 国際標準化機構 (ISO) と国際電気標準会議 (IEC) の第一合同技術委員会 (Joint Technical Committee 1) のこと。
  * 参考: ISO/IEC JTC 2 エネルギーの効率化と再利用に関する規格の策定委員会
  * [ISO/IEC JTC 1/SC 25](https://ja.wikipedia.org/wiki/ISO/IEC_JTC_1/SC_25) ISO/IEC JTC 1/SC 25は、国際標準化を行うISOとIECの合同委員会（ISO/IEC JTC 1）において、情報機器間の相互接続に関する標準化を担当する副委員会(subcommittees)である。
    * WG3: 商用構内配線


* ケーブルの規格

  * [ISO/IEC 11801-1:2017](https://www.iso.org/standard/66182.html) 
  * [https://en.wikipedia.org/wiki/ISO/IEC_11801](https://en.wikipedia.org/wiki/ISO/IEC_11801) WikiPedia(en)
* ケーブル試験

  * [IEC 61280-4-2:2014](https://webstore.iec.ch/publication/5096) シングルモードの試験
  * [IEC 61280-4-1:2009](https://webstore.iec.ch/publication/5095) マルチモードの試験
  * IEC 61280-4-5 MPOケーブルの試験
  * [IEC TC86](https://www.iec.ch/public/miscfiles/sbp/86.pdf)

* 目視検査
  * [IEC 61300-3-35:2015 RLV Redline version](https://webstore.iec.ch/publication/22763)
  * [IEC 61300-3-35:2015](https://webstore.iec.ch/publication/22763) 光ファイバコネクタプラグ及び 光トランシーバのファイバスタブの端面外観検査c)
  * [61300シリーズIEC/JIS対比一覧表](http://www.oitda.or.jp/main/st/61300/61300_170406.pdf)

* [レセプタクル形光トランシーバの光コネクタ端面清掃に関するガイドライン](http://www.oitda.or.jp/main/st/TP12-2.pdf)

* ケーブルテスト用語
  * Tier1(必須)/Tier2(拡張): TIAのテスト用語
  * RTM(必須)/ATM(拡張): IECのテスト用語

* 光ケーブルテスト

  * LPSM: light source and power meter
  * OLTS: optical loss test set
  * 通常はLPSMをする、特性を見る時はOLTSをする。OLTSだけをすることはあまりなくLPSM+OLTSかLPSMのみがほとんど
  * Flukeの場合LPSM用の機器、OLTSの機器があるらしい
　* OLTSはトラブルシュート向き

* MPO
  * Type-A: ストレート、Type-B: クロス、Type-C: 1-2 2-1, 3-4, 4-3..となっているやつ
  * オス・メスがある
  * 12芯が基本、24芯、36芯というのもある、ネットワーク
  * DCレベルでは12芯MPOを使うのが標準的(真ん中4芯は使わない)
  * MMFはコア？がフラットになっており、SMFは斜めにカットされている(らしい)

* テスト用語

  * BERT: Bit Error Rate Testing
  * [ALSNR](https://www.tsuko.co.jp/lan_yogo10.html) Alien Limited Signal to Noise Ratio
  * [既存のケーブル・インフラが 2.5/5GBASE-T をサポートできるか？](https://jp.flukenetworks.com/blog/cabling-chronicles/will-my-existing-cable-plant-support-255gbase-t) ALSNRの解説

  * 2.5/5GBase-TにCat5eやCat6を利用する時は、(1) ケーブル単体の試験と(Internal Parameter、挿入ロス・リターンロス・クロストーク等)と(2) ALSNRの試験が必要
  * ALSNRはTSB-5021で定義されている。


## IEEE802.3:2015

IEEE-802.3:2015 Section1 21 pageより

| Section | Clause  | Annex     |
|---------|---------|-----------|
| 1       |  1 ~ 20 | A ~ H, 4A |
| 2       | 21 ~ 33 | 22A ~ 33E |
| 3       | 34 ~ 43 | 36A ~ 43C |
| 4       | 44 ~ 55 | 44A ~ 55B |
| 5       | 56 ~ 77 | 57A ~ 76A |
| 6       | 78 ~ 95 | 83A ~ 93C |


## 光ケーブルメーカー

| 社名(カタログ) |      |
|----------------|------|
| [住友電工](http://www.optigate.jp/pdf/) | |
| [フジクラ](http://www.fujikura.co.jp/products/optical/opticalfibers/03/2056693_14084.html)  | |
| [古河電工](https://www.furukawa.co.jp/product/catalogue/optical.html) | | 
| [コーニング](https://www.corning.com/jp/jp/products/communication-networks/products/fiber.html) | |
| [CommScope](https://ja.commscope.com) | |


## 各コネクタの電源規格

| Class  | OSFP | QSFP-DD | QSFP28 |
|--------|------|---------|--------|
| class1 | 1.5W | 1.5W    | 1.5W   |
| class2 | 3.5W | 3.5W    | 2.0W   |
| class3 | 7W   | 7W      | 2.5W   |
| class4 | 8W   | 8W      | 3.5W   |
| class5 | 10W  | 10W     | 4.0W   |
| class6 | 12W  | 12W     | 4.5W   |
| class7 | 14W  | 14W     | 5.0W   |
| class8 | >14W | >14W    | 10W    |

* [OSFP Rev2.0](https://osfpmsa.org/assets/pdf/OSFP_Module_Specification_Rev2_0.pdf)
* [QSFP-DD](http://www.qsfp-dd.com/wp-content/uploads/2018/09/QSFP-DD-Hardware-rev4p0-9-12-18-clean)
* [QSFP28](https://members.snia.org/document/dl/25969)
* [OpenEye](https://www.openeye-msa.org)

## その他

* [山本光学 YL-250G](https://www.yamamoto-kogaku.co.jp/safety/product/category03.php)

##

* [Transceiver Slack](https://transceiver.slack.com/join/shared_invite/enQtNTU0MjE2MzMxNjY3LWZlYjA1ZGVlZjNhMjU0NGVhZmUyYmIwNjk0MWExNjI0NjU2YjJkMDRmMGFhM2MyYTMyNDY3NTJkMWJkYTI5OGU)
