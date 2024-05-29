# datavisualization-challenge

## Data Sourcing and Modification

### Data Sourcing
The data consists of two files:
1. **Mouse Metadata**: Information about the mice including their ID, drug regimen, sex, age, and weight.
2. **Study Results**: Results of the study including mouse ID, timepoint, tumor volume, and metastatic sites.

### Data Modification
1. **Reading Data**: Loaded the data into Pandas DataFrames.
2. **Combining Data**: Merged metadata and study results using `Mouse ID`.
3. **Cleaning Data**: Removed duplicate entries.
4. **Filtering Data**: Focused on Capomulin, Ramicane, Infubinol, and Ceftamin regimens.

## Analysis and Figures

### 1. Summary Statistics for Tumor Volume by Drug Regimen
Capomulin and Ramicane show the lowest mean and median tumor volumes.

| Drug Regimen | Mean Tumor Volume | Median Tumor Volume | Tumor Volume Variance | Tumor Volume Std. Dev. | Tumor Volume Std. Err. |
|--------------|-------------------:|--------------------:|----------------------:|-----------------------:|-----------------------:|
| Capomulin    | 40.6757            | 41.5578             | 24.9478               | 4.99477                | 0.329346               |
| Ceftamin     | 52.5912            | 51.7762             | 39.2902               | 6.26819                | 0.469821               |
| Infubinol    | 52.8848            | 51.8206             | 43.1287               | 6.56724                | 0.492236               |
| Ramicane     | 40.2167            | 40.6732             | 23.4867               | 4.84631                | 0.320955               |

### 2. Box Plot of Tumor Volume Distribution
Identified an outlier for Infubinol at around 36.32 mm³.

### 3. Line Plot for Tumor Volume vs. Timepoint for a Single Mouse Treated with Capomulin
Tumor volume decreases over time, indicating the effectiveness of Capomulin.

### 4. Scatter Plot of Mouse Weight vs. Average Tumor Volume for Capomulin
Shows a positive correlation between mouse weight and average tumor volume.

### 5. Correlation Coefficient and Linear Regression Model
Strong positive relationship between mouse weight and average tumor volume, with a high R-squared value.

## Observations and Inferences

1. **Efficacy of Capomulin and Ramicane**: More effective in reducing tumor sizes compared to Infubinol and Ceftamin.
2. **Weight-Tumor Volume Relationship**: Heavier mice tend to have larger tumors on average.
3. **Outlier Identification**: Monitoring outliers can provide insights into unique treatment responses.

## Conclusion
The analysis provides valuable insights into the effectiveness of the Capomulin regimen in reducing tumor sizes. The positive correlation between mouse weight and tumor volume suggests the need for personalized treatment strategies. Monitoring outliers can further enhance the efficacy of drug regimens.

## Code Source
1. Learning Assistant
2. GitHub location: git@github.com:jeffjunohkim/datavisualization-challenge.git