# **MONTHLY PURCHASE PREDICTION FOR E-COMMERCE**
# Olist Brazilian E-Commerce

**Created by :**<br>
Nathania Frieska Zamris (JCDS 0106 002)<br>
Mary Amalia Wauran (JCDS 0106 006)<br>
Idam Ahmadi (JCDS 0106 007)<br>

We are predicting the Total Item Value (TIV) that will occur in the next **4 months** (end of 2018) based on the company's historical data from 2016-2018.
The purpose of making the prediction is to give the marketing team an idea of how much TIV can be achieved by the end of the year and help them determine the **budget** needed to reach that TIV.

Here we also provide some recommendations both from the marketing and non-marketing perspective, based on the data insights we have found, including :

1. How to increase Retention and Average Basket Size (ABS)?
1. What are the performance and potential of the city?
1. What are the potential and obstacles of the best-selling product?
1. How to improve service in line with the increasing number of transactions?
1. Is there any other potential that can be used as product diversification?

We use **Brazilian E-Commerce Public Dataset**
- Source : [kaggle.com](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce?select=olist_products_dataset.csv)
- Authors : Olist and André Sionek
- Year : 2018

**Olist E-Commerce** is a Brazilian online marketplace that connects merchants (small and medium-sized businesses) with customers throughout Brazil. Merchants can use Olist to sell their products online and access a wider market share, logistics services, and payment processing solutions.

We build a model that will help the company provide a purchase prediction tool, which will be useful for determining the marketing budget. Forecasting for the next 4 months will be done by trying modeling using Fbprophet, ARIMA, and Elastic Net. The metric used is MAPE, and the comparison of the graphs between the models will be used for evaluation.

We decided to use MAPE as the evaluation metric for several reasons :
- Our graph has significantly different trends, so using nominal error evaluation of 10000 in 2017 might be large but small in 2018, whereas with MAPE such perception differences can be avoided.
- MAPE is easier to understand for the marketing team.
