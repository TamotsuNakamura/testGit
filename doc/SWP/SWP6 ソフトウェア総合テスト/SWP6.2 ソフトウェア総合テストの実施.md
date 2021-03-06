# SWP6.2 ソフトウェア総合テストの実施

**ソフトウェア総合テストを実施する。**

## 6.2.1 ソフトウェア総合テストの実施

### 入力

[（SW601）](SWP6.1%20ソフトウェア総合テストの準備.md)ソフトウェア総合テスト仕様書  
[（SW603）](SWP6.1%20ソフトウェア総合テストの準備.md)ソフトウェア総合テストデータ  
[（SW602）](SWP6.1%20ソフトウェア総合テストの準備.md)実機  
（SU1002）ソフトウェア開発環境  

### 概要

ソフトウェア総合テスト仕様書に従って、テストを実施する。

### 出力

（SW605）ソフトウェア総合テスト結果

### 実施内容

---

**ソフトウェア総合テスト仕様書に従いテストを実施する。**

1. ソフトウェア総合テストを実施する。
   * ソフトウェア総合テスト仕様書（SW601）をもとに、ソフトウェア総合テストを実施し、出力結果を得る。
   * 代替テストを実施した場合は、理由を明記した上で記録に残す。
   * 不具合検出時、継続して残りのテストを実施するか、不具合が修正されるまでペンディングするかの判断をする。
   * 出力結果を収集する（各種ログなど）。
   * 準備したテスト項目が実施できなかった場合は、理由を明記した上で記録を残す。また、その理由の妥当性について判断する。

1. 修正確認テストを実施する。
   * 不具合が発生し、それを修正した場合の確認として、不具合が解消されたかテストを実施する。
   * 不具合の修正により、別の不具合が発生してないかテストを実施する。

### 注意すべき事項

---

* 修正確認テストでは、修正後の最新版でテストしているかどうかなどを確認する。

<div style="page-break-before:always"></div>

## 6.2.2 ソフトウェア総合テスト結果の確認

### 入力

[（SW601）](SWP6.1%20ソフトウェア総合テストの準備.md)ソフトウェア総合テスト仕様書
[（SW504）](../SWP5%20ソフトウェア結合テスト/SWP5.2%20ソフトウェア結合テストの実施.md)実行可能形式化された最終のソースコード
[（SW605）](SWP6.1%20ソフトウェア総合テストの準備.md)ソフトウェア総合テスト結果
（SU601）不具合管理票（修正確認の場合）

### 概要

テスト結果を確認し、テストの合否を判定する。

### 出力

（SW606）ソフトウェア総合テスト報告書
（SU601）不具合管理票

### 実施内容

---

**ソフトウェア総合テストの結果を確認し、実施したテスト項目の合否を判定する。**

* 不具合を発見した場合、不具合管理票に不具合内容を記録する。
* 修正確認テストの結果、不具合が解消された場合は、修正確認が済んだことを不具合管理票に記録する。

### 注意すべき事項

---

* テスト結果に関しては、ソフトウェア総合テスト仕様書の誤りの可能性についても考慮する。
* 結果の合否判定については、ソフトウェア総合テスト仕様書に記載された判定基準に基づいて行う。
