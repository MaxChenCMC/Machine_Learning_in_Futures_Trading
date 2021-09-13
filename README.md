(unfinished)
# Application

用證交所盤後揭露的現貨買賣超 + 期交所的法人期貨部位<br>
(2 + 4 = 6個特徵值)<br>
預測隔天台指期是紅K棒或黑K棒<br>
![](get_data_from.jpg)
##### 資料來源：[臺灣證券交易所](https://www.twse.com.tw/zh/page/trading/fund/BFI82U.html)／[臺灣期貨交易所](https://www.taifex.com.tw/cht/3/futContractsDate)

使用**隨機森林**的`樣本隨機`＆`特徵隨機`來預測

資料蒐集、特徵工程、因子顯著性排序，交易策略回測、模型評估

資料範圍時間範圍：2019-01-02 ~ 2021-09-10

![df.tail()](#)
df.info()

name | Dtype
---|---
Samples total | 655
Dimensionality | 11
Features | 6, int
Target | Boolean

# Tools
sklearn, requests, BeautifulSoup, pandas, numpy, Randomforest, graphviz, seaborn

<hr>

# Data preparation and Pre-processing
Initial examination of the data showed a total 11 features which numerical features only(no categorical). Before building any machine learning model, it is very crucial for the data to be cleaned in an appropriate format.

# 共線(multi-collinearity)性診斷，資料分佈，特徵轉換
類別字串類需One-Hot Encoding處理(純數值不需處理畢竟決策樹只二分)

# Knowledge Discovery in Database(Data Mining)
Interpretation Evaluation

# 模型評估、調參fine tuning微調、optimeze最佳化, 圖像化漸變的程程
決定深度、截枝與否

# 成果參數回測
Backtesting
