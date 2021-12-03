# Global Superstore Sales Analysis. 
Analysis of Sales of Global Superstore from Profit, Sales, Profit Ratio with Global Superstore Dataset (AHM Data Analyst Technical Test). Global Superstore dataet is contains data on order details of customers for orders of a superstore globally 

## Data Inspection
Global Superstore dataset have 51290 rows and 24 columns, which is included 4 kind of data types like datetime64[ns], float64, int64, object(categorical)
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
luckily the data is clean because there are no missing value and duplicates value, so the data cleansing is removing unnecessary columns such as 'Row ID', 'Order ID', 'Customer ID', 'Postal Code', 'Product ID'

But new column 'Profit Ratio' created by calculation of 'Profit' divided by 'Sales', to measure the profit at ratio

## Exploratory Data Analysis
**DISCLAIMER: his Analysis still just for Providing Insight Purpose. It should be available to proceed to advanced analysis**
### Most Best Sales of Category
![](https://github.com/hendrywijaya98/Global_Superstore_Sales_Analysis/blob/main/images/most_profit_category.png)

Office Supplies are the most profitable, based on Margin Profit of Sales that Office Supplies are the highest

![](https://github.com/hendrywijaya98/Global_Superstore_Sales_Analysis/blob/main/images/most_category.png)


Even Tech is the most Sales and Profit, but IT Still not bring good profit margin to tech


![](https://github.com/hendrywijaya98/Global_Superstore_Sales_Analysis/blob/main/images/most_profitrate_category.png)

Then break it down into Sub-Category, Where the highest is right on Office Supplies Such as Papers and Labels


### Segment with most Profit Ratio
![](https://github.com/hendrywijaya98/Global_Superstore_Sales_Analysis/blob/main/images/most_revenue_segment.png)

The Revenue from segment are close to Equal, It Still Gross Revenue where Shipping Cost are Included

![](https://github.com/hendrywijaya98/Global_Superstore_Sales_Analysis/blob/main/images/most_netprofit_segment.png)

This is The Profit of Sales based, Finally can be discovered where home office are the highest, even there are not significant different

![](https://github.com/hendrywijaya98/Global_Superstore_Sales_Analysis/blob/main/images/most_profitrate_segment.png)

And The Profit Rate, where the Home Office are the highest profit rate, but we need to investigate furthermore 


### Region with The Most Profit
![](https://github.com/hendrywijaya98/Global_Superstore_Sales_Analysis/blob/main/images/most_profitrate_market.png)

Market Area with the most profit rate, Its Fell Right on Canada, Then it followed by United States and Europe Union

![](https://github.com/hendrywijaya98/Global_Superstore_Sales_Analysis/blob/main/images/most_profitrate_region.png)

Profit Rate based on Region, But it doesn’t Show significant difference, even the result still same that canada is the highest

### The Most Profitable of Ship Mode
![](https://github.com/hendrywijaya98/Global_Superstore_Sales_Analysis/blob/main/images/most_sales_shipping.png)

Shipping Mode Number based on Quantity, They’re look like equal, but it’s look like standard are the most even no significant difference  

![](https://github.com/hendrywijaya98/Global_Superstore_Sales_Analysis/blob/main/images/most_profitrate_shipmode.png)

Check it out the Profit Ratio, The Most Profit finally discovered on Second Class,  Followed by Same Day and Standard even they’re slightly difference

![](https://github.com/hendrywijaya98/Global_Superstore_Sales_Analysis/blob/main/images/most_expensive_shipcost.png)

Checking the Shipping Cost, But on the Most Shipping Cost is on Same Day 

### Effect of Discount on Profit
#### Financial features Correlation 
![](https://github.com/hendrywijaya98/Global_Superstore_Sales_Analysis/blob/main/images/finance_corr.png)

It’s looks like discount have negative correlation to Profit

#### Effect of the discount to the Profit Margin
![](https://github.com/hendrywijaya98/Global_Superstore_Sales_Analysis/blob/main/images/discount_effect.png)

But in this chart that, more discount can make profit become less
