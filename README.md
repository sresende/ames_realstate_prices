# Project 2 - Prediction Model for Ames's Properties Sale Price

## Problem Statement
The objective of the project is to develop a regression model to predict the sale price for those who own a property in the Ames area and want to know how much approximate their property worth in case they decide to sell.

The model that will be developed is a linear regression model to predict the sale price of Ames properties considering the main variables and trying to figures out the influence of it in the sale value. 

The metric used to evaluate the performance of this model will be the R2 score, which seeks to reduce the distances between the real value of sales prices and those predicted by the model. 

The developed model will be adjusted using Rigdes and Lasso Regularization to adjust and obtain the best score between it.

This model could also be interesting for real estate companies since it could be used to attract customers in the face of a supposed real estate' appreciation

## Datasets 
In this Project we  analysed datasets related to Ames real state [1]. It contains 2051 records with  detailed information regarding sales made between 2006 and 2010. 

* [`train.csv`](./data/train.csv) | [data dictionary](https://git.generalassemb.ly/sresende/project-2/blob/master/data/dict.txt)
* [`test.csv`](./data/test.csv) | [data dictionary](https://git.generalassemb.ly/sresende/project-2/blob/master/data/dict.txt)



## Data Evaluation

A process of cleaning and evaluating the records was carried out to verify the completeness and consistency of the information. After this cleaning process, we observed how the events behaved according to the sale price during these years.


# ![](https://git.generalassemb.ly/sresende/project-2/blob/master/images/HistogramProperties.png)

The prediction model was built on a sample with a slightly skewed normal distribution followed by a process to remove outliers and other distortions

# ![](https://git.generalassemb.ly/sresende/project-2/blob/master/images/BoxPlotNeighborhoods.png)
Visualizing the sample with these boxplots, we were able to observe which neighborhoods had the most valued properties like Somerst, NridgHt, NoRidge and Crawfor



# ![](https://git.generalassemb.ly/sresende/project-2/blob/master/images/CorrelationsPrice.png)

We could not observe which variables are strongly related to the target of our model. Some of them are inversely proportional like building age


# ![](https://git.generalassemb.ly/sresende/project-2/blob/master/images/ScatterPlotPriceSize.png)
# ![](https://git.generalassemb.ly/sresende/project-2/blob/master/images/ScatterPlotPriceSizeWOutliers.png)
# ![](https://git.generalassemb.ly/sresende/project-2/blob/master/images/ScatterPlotPriceSizeWOutliersLog.png)
Removing outliers and applying transformations in our target (sale price)t.


# ![](https://git.generalassemb.ly/sresende/project-2/blob/master/images/ScatterSeaFeatures.png)

Looking at the other relationships with the target, we could observe that the garage area interferes much more with the target than the lot area and we could still observe in more detail the inverse relationship of the age of the property on the target.



# ![](https://git.generalassemb.ly/sresende/project-2/blob/master/images/ScatterPlotResiduals.png)
# ![](https://git.generalassemb.ly/sresende/project-2/blob/master/images/histogramResiduals.png)

# ![](https://git.generalassemb.ly/sresende/project-2/blob/master/images/lassoCoeficients.png)



##  Recomendations and Conclusions

After analyzing the data, we can see that some variables are more important than others in determining the value of real estate prices. For example, the general condition of the property carries more weight than adding a few feet to the size of the property.

Another conclusion that we can consider is that if you want to add value to the property, it will be more efficient to include one more bathroom than a parking space.


---
References:

[1] [*City of Ames Assessor Site*](https://www.cityofames.org/government/departments-divisions-a-h/city-assessor) 

