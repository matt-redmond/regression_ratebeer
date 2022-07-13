Can we scrape data from the Rate Beer web site and build a predictive model to understand which variables most affect the overall score of the beer on the site.  The website we are using is ratebeer.com.  We will start with ratebeer.com/beerstyles/ to get a list of urls and then iterate through each style to get lists of the urls of individual beers.  Expected features include Average rating, Number of ratings, Number of reviews, IBU, Alcohol by Volume, Location of brewery, age of the beer brand, as well as some features based on words in the reviews.  The target will be the overall score of the beer on the site.

The plan is to use request and Beautiful Soup for webscraping and stats models for linear regression.  Will use pandas and probably Seaborn and Matplotlib for charts.  The MVP should contain some successful preliminary analysis of data successfully scraped from the site.

As an FYI, I initially looked at Beer Advocate but they explicitly say on their website that they do not allow web scraping of any kind.

