# Predicting Wine Quality 🍷

- [Predicting Wine Quality](#predicting-wine-quality)
  - [Introduction](#introduction)
  - [Directory structure](#directory-structure)
  - [Data Processing](#Data-Processing)
  - [Findings](#Findings)
      - [Count vs Quality](#count-vs-quality)
      - [Pie Chart](#pie-chart)
      - [Citric Acid Feature](#citric-acid-feature)
      - [Correlation with Heatmap](#correlation-with-heatmap)
  - [Conclusion](#conclusion)

## Introduction

Created Machine Learning models to predict color of wine from the wine dataset. The dataset can be found from the citations folder. In this project, I have used python libraries such as numpy, pandas, matplotlib, seaborn, scikit learn. 

## Directory structure

The code is stored as a jupyter notebook Wine **quality Prediction-checkpoint.ipynb** inside **src** folder. To run the code, please open the file in jupyter and use run all command to run the code. The data is present at **src/data** location.

## Data Processing

As part of Data Processing to clean the data, the duplicate rows were removed, univariate and multivariate outliers were removed, the skewness in the data was handled using square root transformation, nominal categorical column **color** was one hot encoded

## Findings

#### Count vs Quality

The count plot reveals that there are more average quality wines in comparison to the low and high quality ones.

![Count Vs Quality](https://github.com/nipun1992/Predicting-Wine-Quality/blob/main/pics/count%20vs%20quality.png)

#### Pie Chart

The pie chart highlights the percentage wise distributions of the wines of respective quality levels.

![Pie Chart](https://github.com/nipun1992/Predicting-Wine-Quality/blob/main/pics/Pie%20Chart.png)


#### Citric Acid Feature
![Citric Acid Feature](https://github.com/nipun1992/Predicting-Wine-Quality/blob/main/pics/citric_acid.png)



### Correlation with Heatmap

In the heatmap, if there are any 2 independent features that are highly correlated i.e. 80% or more, then we can drop 1 of those 2 features because both those features are serving the same purpose. We can see that density and 'residual sugar' features have a `pearson correlation coefficient of 0.83` i.e. *83% and thus we can drop 1 of these 2 features*. But in the dataset of red wines, these 2 features are not strongly correlated and thus we cannot drop 1 amongst these 2 features from the red wine dataset.

![Heatmap](https://github.com/nipun1992/Predicting-Wine-Quality/blob/main/pics/heatmap.png)


Hence, We retained the features.

## Conclusion
