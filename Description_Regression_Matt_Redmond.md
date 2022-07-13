Abstract

The goal of this project was to use linear regression to predict the scores of beer at ratebeer.com.  The first step was to webscrape the data from ratebeer.com website.  Next this data was cleaned and put through exploratory data analysis.  Then the data was trained, validate, and tested through a series of linear regression models.

Design

The question for this project is whether the score of a beer can be predicted by using its base attributes.  In the past 10-15 years the variety of beers has increased exponentially.  Beer rating websites have been created to help consumers figure out which beers they may like to try.  Beer brewers are also trying to understand what beers consumers like the most and will be successful in the marketplace.  This project seeks to see if the overall beer score can be understood as a function of it’s key features.  

Data

The dataset contains 6848 beers that were webscraped from ratebeer.com.  There were initially 5 linear features and 20 non-linear features as well as the dependent feature “score”.  Some of the non-linear features could be further grouped into categories.  The data was imported into a pandas data frame and cleaned in python.

Algorithms

20% of the data was held out for testing.  5-fold cross-validation was used for training and validation on the remaining 80%.  Linear regression was used on a base line of just linear features.  Then the non-linear features were added as dummy variables is groups to test their effect.  Once the optimal model using the dummary variables was found, regularization was considered.  Ridge, Lasso, and Elastic Net models were tried but none of them had a positive effect.  Variance Inflation Factor was also considered as a potential issue.  Finally, multi-collinearity led to 2 linear features being discarded.  The best model led to a r-squared value on the test data of .54 with RSME of 12.3.

Tools

Tools used included Requests, BeautifulSoup, pandas, and selenium for webscraping.  Pandas and SciKit-learn were used for modeling.  Seaborn was used for visualizations.


Communication

Slides and visuals presented included a pair-plot and the effect of the non-linear features.  The conclusion was that the model was underfitted and that more data / features were needed to improve the effectiveness of the model.


