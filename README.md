# bike-score-predictor

The objective of this project is to build a model to predict "bikeability" of cities across the United States based on various city features. The use case for this model is a pilot bike and scooter share program looking to expand into a new urban market.  
  
I use OLS regression techniques to predict the target value, urban bike score, which ranges from 0 (poor biking conditions) to 100 (perfect biking conditions). Features for my model include a city's public transit score, population, population density, business density, weather, GDP per capita, and local tax rates. Data sources include Walk Score, U.S. Climate Data, INRIX, City Lab, and the Tax Foundation. 

I assess model performance based on mean absolute error. OLS regression with laso regularization yielded the best results, and predicted city bike scores within an average of 6.3 points of the actual value in the test set. According to the model results, bike-friendly cities are more congested , have a high combined walk and public transit score (i.e. there exists a precedent for alternative modes of transit to private cars), and have relatively nice weather (specifically, low precipitation). 

The results of the project are available in the PowerPoint file "Bike-score-predictor-presentation". My codes are available in a Jupyter Notebook entitled "Bike-score-predictor-notebook" for reproducibility. 

Future work for model improvement include inclusion of additional features likely related to bikability (e.g. existence of bike-friendly infrastructure and level of hilliness). I would also like to utilize classification algorithms to classify cities based on their general level of bikability (e.g. low, medium, or high), rather than OLS regression. Finally, once my model results have been optimized, I would like to expand the scope to include international cities for which bike score indexes are not currently available.
