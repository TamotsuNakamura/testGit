# SWP3.2 ソフトウェア詳細設計の確認

**詳細化された処理が実装可能なレベルであることを確認する。**

## 3.2.1 ソフトウェア詳細設計書の内部確認

### 入力

[（SW205）ソフトウェア・アーキテクチャ設計書](../SWP2%20ソフトウェア・アーキテクチャ設計/SWP2.1%20ソフトウェア・アーキテクチャ設計書の作成.md)
[（SW305）ソフトウェア詳細設計書](SWP3.1%20機能ユニット詳細設計書の作成.md)

### 概要

ソフトウェア詳細設計がソフトウェア・アーキテクチャの設計事項を満たし、かつ、実装可能なレベルか確認し、内部確認レポートとしてまとめる。

### 出力

（SW306）内部確認レポート（ソフトウェア詳細設計）

### 実施内容

---

1. 下記の視点でソフトウェア詳細設計書の内容を確認する。

* 個々のユニットの切り分けの正しさ、および各ユニットの処理内容の明確さ
* ユニット間のインタフェース情報の整合性
* 個々のユニットとハードウェアとの関係

2. 確認結果は内部確認レポートとして整理し、確認作業で指摘された問題およびその対応元を明記した上で関係者に配布する。

### 注意すべき事項

---

* 確認すべき事項としては、以下のようなものがある。

  * プログラムユニット構成の妥当性
  * 機能ユニットとプログラムユニット間の一貫性
  * 機能ユニット間インタフェースの整合性
  * プログラムユニット間インタフェースの整合性
  * メモリ（テーブル、バッファなど）の構造、排他制御、無駄なエリア
  * 各種設定値、引数値（OSシステムコール、汎用ライブラリなど）
  * 高速化が必要な処理は、その実現方法
  * ハードウェア制御方法、設定値
  * ハードウェア機能の効果的利用（処理の高速化などを検討したか）
  * 無限ループ、デッドロック（発生する条件がないか確認する）
  * 割込み処理（多重割り込み、終了処理など）
  * 実装に必要な情報はもれなくソフトウェア詳細設計書に記載されているか

* 管理者は内部確認において指摘された問題事項については、解決策やそのためのアクション（共同レビューの開催など）などもあわせて記載しておくことが望ましい。