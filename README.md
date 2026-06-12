# Mapping Green Space and Happiness in London with Python

An exploratory GIS project using **GeoPandas** to investigate whether London's greener boroughs also report higher levels of happiness. Mental health and green space is a huge topic currently, and I think these results support significant research.

This project was my first real dive into Python's GIS ecosystem, having previously done most of my spatial analysis in R (its better imo, or acrgis/qgis). 
---

## Overview

The project combines two datasets:

* London boroughh boundary shapefiles
* London Borough demographic profiles

Using these data, I explore whether the percentage of green space within each borough is associated with residents' reported happiness.

The workflow includes:

* Reading and plotting GIS shapefiles with GeoPandas
* Cleaning and importing census-style data
* Handling CSV encoding issues
* Joining spatial and tabular datasets
* Producing choropleth maps
* Calculating Pearson's correlation coefficient
* Visualising the relationship with a regression plot

---

## Libraries Used

* GeoPandas
* Pandas
* NumPy
* Matplotlib
* Seaborn
* SciPy
* adjustText
* chardet

---

## Results

After joining the datasets and comparing green space with reported happiness, the analysis found:

* **Pearson correlation:** **0.418**
* **P-value:** **0.0155**

This suggests a **moderate positive relationship** between green space and happiness across London's boroughs, with the result being statistically significant at the 5% level.

While this doesn't imply that green space causes happiness, it does support the idea that greener boroughs tend to report higher levels of wellbeing.

---

## Visualisations

The notebook produces several visualisations, including:

* Choropleth map of green space across London boroughs
* Choropleth map of reported happiness
* Scatter plot with fitted regression line showing the relationship between green space and happiness

---

## Skills Demonstrated

* Geographic Information Systems (GIS)
* GeoPandas
* Data cleaning
* Spatial joins
* Data visualisation
* Statistical analysis
* Correlation testing
* Python

---

## Future Improvements

Some obvious extensions to this project would be:

* Investigating additional predictors of happiness such as income, crime or housing affordability.
* Building a multiple linear regression model rather than examining a single variable.
* Using more recent London Borough Profile data.
* Producing interactive maps with Folium or Plotly.

---

## Author

Created as part of my ongoing effort to become more comfortable using Python for data science and spatial analysis.
