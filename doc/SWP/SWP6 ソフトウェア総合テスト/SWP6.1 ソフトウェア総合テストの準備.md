# SWP6.1 ソフトウェア総合テストの準備

**ソフトウェア総合テストの準備する。**

## 6.1.1 ソフトウェア総合テスト仕様書の作成

### 入力

[（SW105）](../SWP1%20ソフトウェア要求定義/SWP1.1%20ソフトウェア要求仕様書の作成.pdf)ソフトウェア要求仕様書  
テスト仕様書作成に必要な情報（成果物）

### 概要

ソフトウェア総合テスト仕様書を作成する。

### 出力

（SW601）ソフトウェア総合テスト仕様書

<a id = "SW601"></a>

### 参照情報

過去のソフトウェア総合テスト仕様書

### 実施内容

---

**ソフトウェア要求仕様書をもとにソフトウェア総合テスト仕様書を作成する。**

* ソフトウェア要求仕様書に書かれた内容が正しく実現されているか確認するためのテスト項目を準備する。テスト項目としては、ソフトウェアの機能要求、非機能要求などを網羅する形で準備する。
* 個々のテスト項目に関する合否判定の基準を明確にしておく。

### 注意すべき事項

---

* 過去のソフトウェア総合テスト仕様書の再利用について検討する。
* 過去の不具合事例を考慮しているか確認する。
* シリーズ製品の場合、新規機能テスト項目が十分であるか。また、変更機能の影響把握はできてるか確認する。
* 状態遷移表、マトリックス網羅法等を用い、漏れのないテスト項目を抽出する。
* テスト手順や完了条件が、法令、規格等に準拠しているか確認する。
* 想定される出力結果が明確になっているか確認する。
* 実際のエンドユーザの使用状況を考慮したテスト項目を作成する。
* 正常系および異常/例外系のテスト項目を作成する。
* 他システムとの整合やハードウェアとの整合を考慮する。

* **テスト仕様書は、設計フェーズなど上流プロセスの中で検討、作成しておくと良い。**

* **文書化での留意点**
  * 変更履歴を添付し、変更箇所を明示する。
  * 作成文書に関しての責任所在を明示する。
  * 作成文書は構成管理および変更管理にて確実に管理する。

<div style="page-break-before:always"></div>

## 6.1.2 ソフトウェア総合テストの準備

### 入力

[（SW601）](#SW601)ソフトウェア総合テスト仕様書
[（SW504）](../SWP5%20ソフトウェア結合テスト/SWP5.2%20ソフトウェア結合テストの実施.md)実行可能形式化された最終ソースコード  
（SU601）不具合管理票（修正確認の場合）

### 概要

ソフトウェア総合テストを実施するために必要なテストデータやテスト環境を準備する。

### 出力

（SW602）実機  
（SW603）ソフトウェア総合テストデータ

<a id = "SW602"></a>
<a id = "SW603"></a>

### 実施内容

---

**総合テストの実施に必要なデータ、テスト環境などを準備する。**

1. テストデータを作成する。
   * 6.1.1で準備したテスト項目を実行するために必要となるテストデータ（具体的な入力データなど）を作成する。

1. テスト環境を準備する。
   * ソフトウェア総合テストに必要なテスト環境を準備する。
     * テスト治具（通信ターゲット等）を作成する。
     * シミュレーションソフトを作成する。

   * ソースコードを実行可能形式に変換し、半導体メモリに書き込む。
   * メモリや回路などを実装し、実環境で動作させるための実機（あるいは試作機）を調達する。

1. テスト結果の判定基準や、テスト全体の評価基準や完了基準なども用意しておく。
1. 修正確認テスト項目を準備する（修正確認の場合）。
   * 不具合が解消されたこと、また修正により別の不具合が発生していないことを確認するためのテスト項目を準備する。
     * 不具合の内容により、テスト範囲を決定しテスト項目を選択する。

### 注意すべき事項

---

* ソフトウェアとしての全体動作に関して、組み込みソフトウェアの場合、特に異常処理関連などの事象を確認するための、テストデータのバリエーションに留意する。
* テスト治具を用意する場合、その精度は許容範囲内であるかを確認する。
* ハードウェアが正常に動作する環境（ノイズ、電源供給等）であるかを確認する。
* テストするバージョンが正しいバージョンであるか確認する。
* テスト環境に関しては不具合発生時の原因分析などを考慮し、テストの再現性のための工夫をしておく。
* 修正確認テストの準備の留意点
  * テストの実行範囲は影響する部分をすべて網羅しているか
  * テストは基本的に既に作成したテスト項目を再利用する。ただし、修正量が多い場合や、影響範囲が広い場合などは、新たなテスト項目を用意することも検討する。

<div style="page-break-before:always"></div>

## 6.1.3 ソフトウェア総合テスト仕様書の内部確認

### 入力

[（SW105）](../SWP1%20ソフトウェア要求定義/SWP1.1%20ソフトウェア要求仕様書の作成.pdf)ソフトウェア要求仕様書  
[（SW601）](#SW601)ソフトウェア総合テスト仕様書

### 概要

ソフトウェア総合テスト仕様書を確認する。

### 出力

（SW604）内部確認メモ（ソフトウェア総合テスト仕様）

### 実施内容

---

**作成したソフトウェア総合テスト仕様書を確認する。**

* ソフトウェア総合テスト仕様書（SW601）に記載されたテスト項目が、ソフトウェア要求仕様書（SW105）に定義された機能要求、非機能要求を検証する項目となっているかを開発グループ内で確認する。

### 注意すべき事項

---

* 確認すべき事項としては、以下のようなものがある。
  * ソフトウェア規模からみたテスト項目数の妥当性
  * テスト項目の網羅性（ソフトウェア要求仕様書との対応）
  * テスト項目の矛盾/重複
  * ソフトウェア非機能要求の評価基準の妥当性（パフォーマンスなど）
  * エラー処理
  * フェールセーフ処理
  * 期待値

* 開発者がテスト項目を作成している場合は、特にテスト項目の抽出やテストの合否の判定基準などが甘くないか（不十分でないか）注意する。
