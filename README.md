##ハイボールアルコール度数計算ツール

このスクリプトは、ウイスキーとソーダの量をもとに、ハイボールのアルコール度数（ABV: Alcohol By Volume）を計算するツールです。ウイスキーのアルコール度数を40%と仮定して計算を行います。

特徴

変更可能な入力: ウイスキーとソーダの量（ミリリットル単位）を自由に指定可能。

エラー処理: 無効な入力や不足しているデータを検出し、適切なエラーメッセージを表示。

正確な計算: 計算結果を小数点以下2桁まで表示

必要条件
Python3

使用方法

1. スクリプトを highball_calculator.py として保存します。


2. 以下の手順でスクリプトを実行します。

python highball_calculator.py


3. スクリプト実行後、ウイスキーとソーダの量を入力します。


4. ハイボールのアルコール度数が計算され、結果が表示されます

入力例
ウイスキーの量を入力してください（ml）: 50
ソーダの量を入力してください（ml）: 150

出力例
ハイボールのアルコール度数は 10.00% です。

注意事項
ウイスキーのアルコール度数は40%で計算しています。
他のアルコール飲料を使用する場合は、スクリプトを修正してください。
