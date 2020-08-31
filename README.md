# Kepler Exoplanet Analysis
The data for this project has been acquired from Kaggle competitions (https://www.kaggle.com/nasa/kepler-exoplanet-search-results) which specifies the objects and their characterstics as perceived by the Kepler space telescope whether the objects are exoplanets or not. The data contains a list of objects, a list of confidence scores which tell the confidence level of an object for being a potential candidate or a false positive, a list containing period of transits, duration of observation, and intrinsic properties of the parent star and the object orbiting around.

### Code and resources
**Python version** : 3.7.6  
**Packages used** : pandas, missingno, scikit-learn, seaborn  
**Reference** : https://exoplanetarchive.ipac.caltech.edu/docs/API_kepcandidate_columns.html  

### Steps
1. Looked out for the missing values in the raw data.
2. Dropped the columns that were not necessary in the analysis.
3. Dropped the objects in the data frame momentarily to replace the missing values with the average of the respective columns using simple imputer.
4. Concatenated the object columns that were dropped earlier.
5. Created a cleaned data file.
6. Exploratory data analysis.

### Plots
The plots below show the number of false positive, candidates and confirmed objects in literature (1st plot) and using observations (2nd plot).  
![in literature](In_literature.png) ![in observ](In_observation.png)  
The confidence score plot below shows that there is a very low confidence for an object being a false positive, which means that most of the objects should probably be planets.  
![confidence](confidence_score.png)  
The heat map shows the correlation of certain columns and how can these columns be used to derive some characteristics of the planets (for example - positive correlation between star temperature and temperature of the planet).  
![heat map](correlation.png)  
The distribution of the radii of the planets (in Earth radii) falls mostly between 0 and 25. There are very few planets that are couple hundred times larger. The size of the parent stars fall between 0 and 25 (almost all).  
![planet](prad_dist.png) ![star](srad_dist.png)  
