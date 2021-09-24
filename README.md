# Global_Superstore_Sales_Analysis
Analysis of Sales of Global Superstore from Profit, Sales, Profit Ratio with Global Superstore Dataset (AHM Data Analyst Technical Test)

## Data Inspection
Global Superstore dataset contain 51290 rows and 24 columns, which is included 4 kind of data types like datetime64[ns], float64, int64, object(categorical)
```
<class 'pandas.core.frame.DataFrame'>
RangeIndex: 51290 entries, 0 to 51289
Data columns (total 24 columns):
 #   Column          Non-Null Count  Dtype         
---  ------          --------------  -----         
 0   Row ID          51290 non-null  int64         
 1   Order ID        51290 non-null  object        
 2   Order Date      51290 non-null  datetime64[ns]
 3   Ship Date       51290 non-null  datetime64[ns]
 4   Ship Mode       51290 non-null  object        
 5   Customer ID     51290 non-null  object        
 6   Customer Name   51290 non-null  object        
 7   Segment         51290 non-null  object        
 8   City            51290 non-null  object        
 9   State           51290 non-null  object        
 10  Country         51290 non-null  object        
 11  Postal Code     9994 non-null   float64       
 12  Market          51290 non-null  object        
 13  Region          51290 non-null  object        
 14  Product ID      51290 non-null  object        
 15  Category        51290 non-null  object        
 16  Sub-Category    51290 non-null  object        
 17  Product Name    51290 non-null  object        
 18  Sales           51290 non-null  float64       
 19  Quantity        51290 non-null  int64         
 20  Discount        51290 non-null  float64       
 21  Profit          51290 non-null  float64       
 22  Shipping Cost   51290 non-null  float64       
 23  Order Priority  51290 non-null  object        
dtypes: datetime64[ns](2), float64(5), int64(2), object(15)
memory usage: 9.4+ MB
```
luckily the data is clean because there are no missing value and duplicates value

## Exploratory Data Analysis
### Most Best Sales of Category
### Segment with most Profit Ratio
### Region with The Most Profit
### The Most Profitable of Ship Mode
### Effect of Discount on Profit
