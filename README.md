# Binary_Classification_Bank_Note_Forgery

## The Data

##### Taken from https://archive.ics.uci.edu/ml/datasets/banknote+authentication.
##### This data set contains data extracted from images that were taken from genuine and forged banknotes. For digitization, an industrial camera usually used for print inspection was used. The final images have 400x 400 pixels. Due to the object lens and distance to the investigated object gray-scale pictures with a resolution of about 660 dpi were gained. Wavelet Transform tool were used to extract features from images.

## EDA

##### 1) Looked at the counts of how many banknotes are forgeries and how many are not
##### 2) Looked at the correlation between whether or not the banknote is a forgery and each of the variables in the dataset
![](https://github.com/savyrosea/Binary_Classification_Bank_Note_Forgery/blob/main/pictures/Heatmap.PNG)
##### 3) Looked at the average value of each variable broken up by whether or not the banknote was a forgery
![](https://github.com/savyrosea/Binary_Classification_Bank_Note_Forgery/blob/main/pictures/means.PNG)
##### 4) Decided to try machine learning with and without the Entropy_of_Image variable to see which model has a higher accuracy.

## Binary Classification Using Logistic Regression

##### Using sci-kit learn, I split my data into testing and training sets, and ran Logistic Regression model to predict whether the bank notes in my training set were forged or not.
##### I repeated this process first with all 4 variables in the data set. Then again by removing the Entropy Variable (the variable I had identified as having the least impact on forgery).
##### Both models predicted with an accuracy of 100% (hmmm, almost works too well...) with my testing/ training data.
##### I also used sci-kit learn to determine the percent chance that the banknote is a forgery or not as well as the prediction whether or not the note is a forgery.

![](https://github.com/savyrosea/Binary_Classification_Bank_Note_Forgery/blob/main/pictures/percents.PNG)
