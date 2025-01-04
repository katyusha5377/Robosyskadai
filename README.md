# ハイボールのアルコール度数計算ツール

[![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)

[![test](https://github.com/katyusha5377/Robosyskadai/actions/workflows/test.yml/badge.svg)](https://github.com/katyusha5377/Robosyskadai/actions/workflows/test.yml)

このプログラムは、ウィスキーとソーダの混合比に基づいて、ハイボールのアルコール度数（ABV）を計算するためのツールです。
ウィスキーの量とソーダの量を入力すると、ハイボールのアルコール度数を正確に算出します。

## プログラムの概要
このツールは、ウィスキーとソーダの総量に対するアルコール量の割合を求め、その結果をアルコール度数（％）として表示します。ウィスキーの量が多ければアルコール度数も高く、逆にソーダが多ければ度数は低くなります。

## 必要な環境
- Python 3.x がインストールされていること
- このプログラムには外部ライブラリは必要ありません。標準ライブラリのみを使用しています。

## 使用方法

### 1. プログラムを実行する

端末（ターミナル）で次のコマンドを入力して、プログラムを実行します：

```python3 highball_abv_calculator.py```

### 2. 入力形式
プログラムは、標準入力からウィスキーとソーダの量（ml）を入力として受け取ります。ウィスキーとソーダの量をスペースで区切って入力してください。

例：
50 150

この例では、ウィスキーが50ml、ソーダが150mlであることを示しています。

### 3. 結果の出力
プログラムは、入力されたウィスキーとソーダの量に基づいて、ハイボールのアルコール度数（ABV）を計算し、その結果を表示します。例えば、入力が「50 150」の場合、次のような結果が出力されます：

ハイボールのアルコール度数: 13.33%

この出力は、ハイボールのアルコール度数が13.33%であることを意味しています。

エラーハンドリング
プログラムは、次のようなエラーを適切に処理します：

入力が空の場合
ユーザーが入力を何も提供しない場合：
無効な入力: 入力が空です

入力の形式が間違っている場合
数値が1つしか入力されていない、または適切に区切られていない場合：
無効な入力: 50

ウィスキーやソーダの量がゼロの場合
ウィスキーやソーダの量が0の場合、アルコール度数の計算ができないためエラーが発生します：
エラー: 全体の量が0です

不正な数値が入力された場合
数字以外の文字が入力された場合など：
エラー: 入力に無効な値が含まれています


プログラムの内部構造

主要関数

1. ```calculate_alcohol_concentration(whiskey_amount, total_amount)```

ウィスキーの量とハイボールの総量からアルコール度数を計算します。

計算式は次の通りです：

ABV = (ウィスキーの量 / ハイボールの総量) * 40

ここで、アルコール度数は通常40%のウィスキーを使っている前提となります。

2. main()

標準入力からデータを取得し、ウィスキーとソーダの量をパースして、calculate_alcohol_concentration関数を呼び出して結果を計算します。
エラーハンドリングと入力確認もこの関数内で行っています。


## 動作環境
### ・テスト済みバージョン: 3.7~3.10
### ・Ubuntu 22.04 LTS

## ライセンス
このプロジェクトは BSD 3-Clause License のもとで公開されています。

© 2024 Yuma Hirano　平野悠真
