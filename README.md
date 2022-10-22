#Retail Sales Prediction

I dealt with the past data of Europe Drug stores in this project and the dataset name was "Rossmann Store"

Sales forecasting plays an integral role in setting expectations and making plans for your business. It’s your best shot at predicting the future. Rossmann operates over 3,000 drug stores in 7 European countries. Currently, Rossmann store managers are tasked with predicting their daily sales for up to six weeks in advance. You are provided with historical sales data for 1,115 Rossmann stores. The task is to forecast the "Sales" column for the test set.

I performed an exhaustive analysis in order to gain insights and engineer features with an interactive exploratory analysis and finally will use different algorithms to predict.
![image](https://user-images.githubusercontent.com/110169716/197323479-f8226d68-0079-4fb7-82f8-02a39a3e3f63.png)

#Columns in the dataframe:

Id - an Id that represents a Store within the test set

Store - a unique Id for each store

Sales - the turnover for any given day (this is what you are predicting)

Open - an indicator for whether the store was open: 0 = closed, 1 = open

StateHoliday - indicates a state holiday. a = public holiday, b = Easter holiday, c = Christmas, 0 = None

SchoolHoliday - indicates if the Store on a particular Date was affected by the closure of public schools

StoreType - differentiates between 4 different store models: a, b, c, d

Assortment - describes an assortment level: a = basic, b = extra, c = extended

CompetitionDistance - distance in meters to the nearest competitor store

CompetitionOpenSince[Month/Year] - gives the approximate year and month of the time the nearest competitor was opened

Promo - indicates whether a store is running a promo on that day

Promo2 - Promo2 is a continuing and consecutive promotion for some stores: 0 = store is not participating, 1 = store is participating

Promo2Since[Year/Week] - describes the year and calendar week when the store started participating in Promo2

PromoInterval - describes the consecutive intervals Promo2 is started, naming the months the promotion is started anew. E.g. "Feb,May,Aug,Nov" means each round starts in February, May, August, November of any given year for that store

#After Exploratory data Analysis, I used different Regression algorithms for training the model

All of the weekday has a promotion and the weekend has no promotion.

The sales price has the highest when there is a promotion.

All Type ‘b’ stores have comparatively higher sales and it mostly constant with peaks appears on weekends.

Majority of Stores remains closed on state holidays.

School holiday increases the sales price and customers proportionally.

Random Forest Regressor is the best for this Dataset Problem.
