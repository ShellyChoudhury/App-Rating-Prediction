# APP Rating Prediction using Machine Learning technique Linea Regression Model building in Python(Pandas,Numpy, Matplotlib,
## Objective
Developed a Machine Learning model to predict the Google apps which have high ratings.

## Problem Statements
Google Play Store team is about to launch a new feature wherein, certain apps that are promising, are boosted in visibility. The boost will manifest in multiple ways including higher priority in recommendations sections (“Similar apps”, “You might also like”, “New and updated games”). These will also get a boost in search results visibility. This feature will help bring more attention to newer apps that have the potential.

## Analysis
Identified  the apps those are promising and boosted visibility. High App ratings,  provided by the customers, have been a  great indicator for predicting the apps ratings.

## Steps Involved
1. **load the data**
2. **check the null values**
3. **drop the null values**
4. **formatting the datatypes for the correct model  building**
5. **Sanity Check**

Average rating should be between 1 and 5 as only these values are allowed on the play store. Dropped the rows that have a value outside this range.
Reviews should not be more than installs as only those who installed can review the app.
For free apps (type = “Free”), the price should not be >0. Dropped any such rows.

6. **Univariate Analysis**
7. **Outlier Treatment**
8. **Bivariate Analysis**
9. **Data preProcessing**
10. **Train the data**
11. **Model Buildinhg**
12. **Making Prediction on test set** 

## Performing Univariate Analysis
**Boxplot for Price**
![output_42_1](https://user-images.githubusercontent.com/107675917/195637142-747cc02a-a891-4fc6-a8cc-409e0daafb38.png)
**Boxplot for Reviews**
![output_44_1](https://user-images.githubusercontent.com/107675917/195637565-67d9bf80-432c-470f-a16e-afc7cf2c7ef6.png)
**Histplot for Rating**
![output_46_0](https://user-images.githubusercontent.com/107675917/195637820-c3e591ce-a666-4ab0-adb2-bf170fed79ec.png)
**Histplot for Size**
![output_48_0](https://user-images.githubusercontent.com/107675917/195638151-e036dd36-25ca-4967-8865-17c9556091c3.png)

## Outlier treatment
Looking for suspicious data.
Deciding  a threshold as cutoff for outlier and dropping  records having values more than that.

## Bivariate Analysis
**Joint plot for Rating vs Price **

![output_66_2](https://user-images.githubusercontent.com/107675917/195846565-953d24bd-ba24-4f29-bc2b-1689bb9f4f64.png)

**Joint plot for Size vs Rating **

![output_67_2](https://user-images.githubusercontent.com/107675917/195847157-d5ffbedd-8870-440d-953a-fc6d1b090061.png)

**Joint plot for Review vs Rating **

![output_69_2](https://user-images.githubusercontent.com/107675917/195847535-ea62cb09-234f-4c3c-867f-fc228369abbe.png)

**Box plot for Rating vs Content writing**

![output_71_2](https://user-images.githubusercontent.com/107675917/195847921-09db0b37-deed-4ff2-a87e-fcc654f6ebd8.png)

**Box plot for category vs Rating**

![output_73_2](https://user-images.githubusercontent.com/107675917/195848194-fc7df6ed-cce8-4feb-856e-da9bcabc7dec.png)

## Data pre-processing

Data pre-processing involves:
1.**Making a copy of the dataframe**
2.**Log tranformations** 
3.**Dropping unneeded columns**
4.**Dummy Encoding**
    
This is important for model building as Machine Learning models can't process categorical data. All data columns before model building should be numeric.
    
## Spliting daat into train and test
The procedure is used to estimate the performance of Machine Learning algorithm when the are used to make prediction on data.


