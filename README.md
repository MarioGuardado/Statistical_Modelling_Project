# Final-Project-Statistical-Modelling-with-Python

## Project/Goals
The goals of the project are to find meaningful correlations and regressions, between public bike stations in the city of Richmond, Virginia, and the characteristics of businesses near them. This goal can be achieved by manipulating information about businesses and bike stations retrieved from online APIs.

## Process
1. Creation of Yelp and Foursquare user accounts.
2. Retrieving relevant information about bike stations from CityBikes and about businesses close to them from Yelp and Foursquare, using their respective APIs.
3. Performing exploratory data analysis and cleaning of the data retrieved from APIs.
4. Creation of a database containing all the cleaned information.
5. Selecting the relevant columns and merging them to create a working dataframe on which to perform statistical analysis and modelling.
6. Exploration of the resulting dataframe using data visualization techniques
7. Construction of a Linear Regression model to illustrate the relationship between the number of bikes in the bike stations and the characteristics of the businesses around them.
8. Review of the output of the model and removal of irrelevant business characteristics to improve the predictive power of the model.


## Results
ߦ Yelp and Foursquare return almost identical information about businesses. However, Yelp returns around 4 times more results than Foursquare, and also returns the user rating and 'price' level of each business, making Yelp a much better option for statistical modelling.

ߦ Of all the available business characteristics, only the number of Yelp reviews has any significant correlation to the total number of bikes in the nearest bike station. However, the regression model returned an Adjusted R-squared value of 0.008, which indicates that the predictive power of the model is minimal.

ߦ Regardless, the following can be inferred: The number of Yelp reviews of a business is likely correlated to the popularity of the business, meaning the number of regular patrons served. Then, there must be an elevated transit of patrons near popular businesses, thus more bikes are required to meet the demands of patrons when compared to areas with less popular businesses.

## Challenges 
A few challenges faced during this project were:
ߦ Information retrieved from each APIs has different formatting, thus a different strategy is required to parse and convert each data set to a dataframe.
ߦ The Correlation of each business to its nearest bike station was not available from the API data and required the use of search algorithms.
ߦ In the yelp_foursquare_EDA.ipynb notebook, the task "Get the top 10 restaurants according to their rating" required the categorization of each venue into categories like 'Restaurant', 'Bar', 'Museum', etc. This is in essence a very time-consuming task.

## Future Goals
Obtaining data from additional sources/APIs to find more meaningful relationships and/or improve the predictive power of the current model.
