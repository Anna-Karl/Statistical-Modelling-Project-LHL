# Final-Project-Statistical-Modelling-with-Python

## Project/Goals
The primary objective of this project is to establish a connection with the CityBike, Yelp, and Foursquare APIs to extract data for chosen city (Como, Italy). The project aims to uncover the relationship between the number of bikes available at specific locations and the characteristics of nearby points of interest. 

## Process
### step 1 - Connecting to CityBikes API
Explored the CityBikes API structure and connected to it. Selected a city and query the API to retrieve bike station data. For each bike station, obtained latitude, longitude, and bike count information. Converted the API responses into a Pandas dataframe.
### step 2 - Connecting to Foursquare and Yelp APIs
Accessed the Foursquare and Yelp APIs to retrieve point of interest (landmarks, historical buildings, arts, entertainment, and active life) data for the same area. Created separate dataframes for Yelp and Foursquare results. Evaluated the quality of information provided by each API for your location, considering various factors.
### step 3 - Joining Data
Merged the CityBike, Foursquare, and Yelp dataframes into a single dataset for analysis. Performed data cleaning on the CityBike, Foursquare, and Yelp. Utilized data visualization techniques to explore and gain insights from the merged dataset. Designed and created an SQLite database to store the collected data. Validated the data in the SQLite database to maintain data integrity.
### step 4 - Building a Model
Built a regression model, to estimate the number of bikes assigned to a station based on station attributes and nearby POI features.
The results of the regression model derive insights from the coefficients and statistical tests. Used the results from the analysis and prediction to demonstrate insights into how POI characteristics impact bike availability.

## Results
The Foursquare API provided a richer set of locations and associated details compared to Yelp. However, it's important to note that many of these locations exhibited significant variability in the number of reviews they had. This variability introduced inaccuracies in the outcomes of the regression model.

Consequently, the results of the regression analysis indicate that the model's ability to explain the variance in the number of available bikes is relatively limited. It suggests that there could be other unaccounted factors influencing bike availability. To enhance the model's predictive accuracy, further exploration and potentially the inclusion of additional variables are necessary.

## Challenges 
Throughout the project, several challenges were encountered, spanning data parsing, cleaning, API handling, timing issues, duplicate points of interest, verticality considerations, database transformation. As well, the data collected at specific times notalways reflect actual bike availability.

## Future Goals
Allocate more time for in-depth (EDA) to uncover additional insights and patterns in the data. Explore relationships between variables and perform more advanced visualizations.

Investigate alternative APIs that may offer more extensive and reliable information. This could potentially improve the quality of data used for modeling.

Explore advanced data visualization techniques, such as circular histograms, to represent data based on various variables like the source of the data, venue category, or other relevant factors. 

Refine the regression model by incorporating additional relevant variables, optimizing hyperparameters, or exploring different modeling techniques.
