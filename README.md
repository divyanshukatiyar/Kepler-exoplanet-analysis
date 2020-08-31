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
The plots below show the number of false positive, candidates and confirmed objects in literature.  
![in literature](\In_literature.png)
