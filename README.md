# Daily-Range-Before-and-After-Earnings-Announcement
Edward O. Thorp, the mathematician, originial balckjack card counter and later successfull hedgefund manager, talked about waiting for rich opportunities before he took on risk. Large daily ranges are rich opportunities which explains why I always did well trading during earnings seasons. I wanted to visualize the expansion in range after an earnings announcement. I choose the companies in sp500 somewhat arbitrarily and I choose 2012-2019 because those were low volitilty years and I didn't want the broader market volatility affecting the results. 

1.CLEAN DATA
  Remove unneeded columns
  Check for Null
  Alter Columns to correct data type
  Check for Outliers 
2. AGGREGATIONS
  Calculate daily range
  Join earnings table and sector
  Lead 5 days Lag 5 partition by ticker
  Bump days forward or back with dailyrange% depending on pre or post (days daily range with pre release times counting the current date as day 1 and post release times counting     the current date as - 1 partition by ticker)
  Average of each day total
  Count dailyrange distribution for day(-2) through (+2)
