# Popularity of Etsy Listings #

## Motivation ##

What makes a product listing popular? Every online marketplace is a complex space with its own set of rules, but it's possible to gain insights by taking a look at the listing features themselves. 

This exploratory data analysis will examine the characteristics of listings on Etsy to gain an understanding of any interesting relationships that may contribute to a post's popularity. Insights could help shop owners create listings that will get the most views and favorites, eventually leading to purchase funnel conversions and increased revenue.

## Data ##

Data for listings and seller taxonomy was extracted from Etsy using the public API. A preview of the data before and after feature engineering can be found in 'fakedata.csv' and 'fakedata_beforecleaning.csv'. 

The final dataset includes features such as:
- product category
- title word count
- description word count
- tag count
- views
- favorites
- month of post creation


<img src="product categories reg.png" width="425"/>


## Defining Popularity ##

Popularity is defined in terms of views and favorites. These two are not perfectly correlated, which makes sense since a favorite indicates deeper engagement than a view. I account for this by dividing the original dataset into 6 separate dataframes, 3 for both, 1 for each level of popularity.


<br>
<br>
<img src="toysgames regular.png" width="425"/>
<img src="toysgames mostpopular.png" width="425"/>
