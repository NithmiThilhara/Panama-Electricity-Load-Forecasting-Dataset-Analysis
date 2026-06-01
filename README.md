# Panama-Electricity-Load-Forecasting-Dataset-Analysis
Explores the application of three powerful multivariate techniques, Principal Component Analysis (PCA), Factor Analysis(FA) and Canonical Correlation Analysis (CCA) on the Panama Electricity Load Forecasting dataset using python.

## Conclusion
- PCA shows that 6 principal components retain nearly all of the dataset’s variance (> 90%). This means we can reduce the 17 numeric dimensions down to 6 for visualization or faster downstream modeling without losing significant information.
- Factor Analysis confirmed a meaningful latent structure in the dataset. Three factors were retained, and these factors were interpretable as a temperature-demand factor, a humidity/cloud factor, and a wind-related factor.
- CCA demonstrated that the strongest relationship between the two predefined sets occurred between the weather variables and the demand/calendar variables.
- In my study, results suggest that electricity demand and calendar effects are meaningfully connected to weather conditions, especially temperature.
- Overall, the analysis shows that the dataset can be reduced to a few major dimensions. The findings also indicate that the main sources of variation in the dataset are associated with temperature, moisture/cloud conditions, and wind, and that weather variables have a clear multivariate relationship with national electricity demand.

## Limitations
- Assumes linearity in data relationships, so nonlinear relationships between weather and electricity demand may not be fully captured.
- Interpretation is complex, especially with multiple canonical variables.
- Factor interpretation depends partly on researcher judgment, especially when assigning labels.
- Outliers were handled cautiously, extreme values in weather and demand data may still influence the extracted components and factor loadings.
- Assumes equal covariance matrices across classes (violations reduce accuracy).
