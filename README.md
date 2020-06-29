# supervised_learning

教師あり学習（単回帰分析・重回帰分析）の学習・統計グラフ分析になります。




# 使用言語 & ライブラリ

Python3, Jupyter Notebook, Numpy, Pandas, Matplotlib, Scikit-learn

## 単回帰分析

傾き$a$の計算式

$$
a = \dfrac{\displaystyle{\sum_{n=1}^{N}}x_{n}y_{n}}
{\displaystyle{\sum_{n=1}^{N}}x_{n}^{2}}
$$

<img width="1234" alt="スクリーンショット 2020-06-27 14 24 01" src="https://user-images.githubusercontent.com/50135286/85981626-7a7d3580-ba1f-11ea-9790-0390bb0f47ad.png">

単回帰分析による家賃の内挿予測値算出です。

○ 計算・手順等

　
⓪ 変数

広さ: x, 家賃: y, パラメータ: a, b, 予測値(predict): ^y
　

① モデル決定

 ^y = ax + b

　
② データの中心化(値より平均値を引き、原点移動により切片パラメータを除外)

xc = x - ￣x

yc = y - ￣y

　
③ 評価関数L（損失関数）決定

L = Σ(yn - ^yn)^2

 ※ nはサンプル数, Σはプログラム上はsum関数を使用

　
③ 評価関数を最小化（微分から傾きa = 0に）

a = (Σxn * yn) / (Σ xn^2)

　
④ 欲しい値(ex. 広さx = 30の家賃)の予測値^yの算出

^y = ax

　　
  
## 重回帰分析

$\boldsymbol{w} = (\boldsymbol{X}^{T}\boldsymbol{X})^{-1}\boldsymbol{X}^{T}\boldsymbol{y}$

![image](https://user-images.githubusercontent.com/50135286/85982627-22dfc980-ba21-11ea-9f6e-9dac95a5b9b6.png)

統計学学習後に補足予定（2020/06/29現在）

