# Data_Analytics_Hw3
S&amp;P prediction
preprocessing 我將今天的收盤價跟隔天的收盤價對比，新增一個欄位如果是上漲的話則為1下跌則為0
作為我資料的y值，利用三種方法來預測隔天的股價是漲是跌
而資料在使用模型之前要先標準化才可以帶入模型
而三種方法中NN的精準度最高但也只有53%的準確度
基本上NN比起前兩種方法只要是資料量夠大
都會比前兩種方法還要準
而要如何增加準確度
我認為可以根據開盤價 最高價格 最低價格 以及收盤價這四個交易的資訊來計算RSI值以及K線圖來增加feature

