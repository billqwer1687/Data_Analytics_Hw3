# Data_Analytics_Hw3
S&amp;P prediction
preprocessing 我將今天的收盤價跟隔天的收盤價對比，新增一個欄位如果是上漲的話則為1下跌則為0作為我資料的y值，利用三種方法來預測隔天的股價是漲是跌，而資料在使用模型之前要先標準化才可以帶入模型，而三種方法中NN的精準度最高但也只有53%的準確度，基本上NN比起前兩種方法只要是資料量夠大，都會比前兩種方法還要準，而SVM如果資料太過龐大或者要分析的種類過多時，他所需要的運算就會呈現指數性的成長，NN則可以透過layer層萃取出feature再加以加工，最後將之flatten進行分類，而分類的行為就很像投票，大家會投票決定此資料隸屬於哪一類，因此當你的樣本數越多時投票數越多發生錯誤的機率就越低(高雄市長是個例外的例子QQ)，而NN與Logistic regression都有可能會發生overfitting，所以在使用時也要特別小心。而要如何增加準確度，我認為可以根據開盤價、最高價格、最低價格以及收盤價這四個交易的資訊來計算RSI值以及K線圖來增加feature，建立RSI值如果值大於80的話就可能會有買超的狀況，因此接著迎接的可能就是股票的下跌，而跌破20就可能是賣超的狀況，K線圖可以依照他的類型又分成好幾種，這些都可以當作參考的feature，單純只從這四個數字模型是沒有辦法幫我們判斷這些東西的，因此我們需要用自己的知識去增加feature提供我們模型更多參考的資料來提高模型的精確度。

