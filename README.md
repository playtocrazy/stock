# Crazy Stock Analytics

# API
+ TWSE API (realtime)  
 api url:   
 `http://mis.twse.com.tw/stock/api/getStockInfo.jsp?ex_ch=tse_2330.tw|otc_3293.tw&json=1&delay=0&_=1435210928008`  
> note: please hit official website (http://mis.twse.com.tw/stock/index.jsp) first to avoid the api response fail.  
> maximum 99 stock number for one request

 reference:
 1. https://github.com/Asoul/tsrtc
 2. https://sites.google.com/site/kentyeh2000/zheng-jiao-suo-ji-shi-zi-xun-jie-xi
 3. http://kentyeh.blogspot.tw/2015/07/blog-post_16.html

+ Yahoo Finance API (realtime)   

        $.ajax({
          url: "http://finance.yahoo.com/webservice/v1/symbols/" + tickers + "/quote?format=json&view=detail",
          dataType: "jsonp",
          jsonp: "callback",
          jsonpCallback: "quote"
        });
        quote = function (data) {
          console.log(data);
        };
api url: `http://finance.yahoo.com/webservice/v1/symbols/2330.TW/quote?format=json&view=detail`  
reference: [Stock-Ticker-Real-Time-Yahoo](https://github.com/ovnisoftware/Stock-Ticker-Real-Time-Yahoo/)

+ Historical API by Yahoo & [project yahoo-finance](https://github.com/pilwon/node-yahoo-finance)
+ Push Notifications to User
reference:  
 1. https://github.com/realtime-framework/ChromePushNotifications
 2. https://github.com/gauntface/simple-push-demo
 3. https://github.com/raix/push
