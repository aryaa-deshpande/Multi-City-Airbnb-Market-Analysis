# Multi-City Airbnb Market Analysis

The goal was to analyze Airbnb listing data from four different cities and compare patterns across markets using PCA and K-Means clustering.

The four datasets included:
```
- Portland, OR
- Pacific Grove, CA
- Albany, NY
- Bozeman, MT
```

All of the code, plots, and analysis are inside the Jupyter notebook:

`Deshpande_AryaaParesh_takehome.ipynb`




## In the notebook:

### 1. Preprocessing

I cleaned and standardized 16 numeric features required by the assignment. This included:
```
	•	converting price strings to numeric values
	•	parsing bathrooms_text into floats
	•	filling missing values with medians
	•	clipping outliers (1st–99th percentile)
	•	scaling everything with StandardScaler
```

All four cities go through the exact same preprocessing pipeline.

### 2. PCA Analysis

For each city:
```
	•	PCA was run on the standardized data
	•	scree plots were generated
	•	number of components needed for 90%+ variance was computed
	•	top feature loadings for PC1 + PC2 were interpreted
	•	cross-city PCA patterns were compared
```

### 3. K-Means Clustering

Using only the first two PCs:
```
	•	the elbow method was used to choose k
	•	silhouette scores were calculated
	•	clusters were visualized for each city
	•	each cluster was interpreted
	•	clustering patterns were compared across cities
```

### 4. Final Conclusions

The notebook ends with a summary of what PCA and K-Means reveal about how these four Airbnb markets are similar and different.



## How to run

jupyter notebook `Deshpande_AryaaParesh_takehome.ipynb`

Then restart the kernel and run all cells from the top.
