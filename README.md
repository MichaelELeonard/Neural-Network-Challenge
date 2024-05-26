# Week 21 Challenge – Deep-Learning
#Preprocessing
## Import and read the charity_data.csv
## Drop the non-beneficial ID columns, 'EIN' and 'NAME'
## Determine the number of unique values in each column
## Look at APPLICATION_TYPE value counts to identify and replace with "Other"
## Choose a cutoff value and create a list of application types to be replaced use the variable name `application_types_to_replace`
## Choose a cutoff value and create a list of classifications to be replaced use the variable name `classifications_to_replace`
## Convert categorical data to numeric with `pd.get_dummies`
## Split our preprocessed data into our features and target arrays
## Create a StandardScaler instances
## Fit the StandardScaler
## Scale the data

# Compile, Train and Evaluate the Model
## Define the model - deep neural net, i.e., the number of input features and hidden nodes for each layer.
## Compile the model
## Train the model
## Evaluate the model using the test data
## Export our model to HDF5 file

### Summary



<img src="ReadMe Pics/Pic 12.png" width="648" height="391">




<br>
<img src="ReadMe Pics/Pic 5.png" width="317" height="74">


<img src="ReadMe Pics/Pic 18.png" width="489" height="177">
<br>

### Overview of the analysis



### The Results


### Summary
Some trends can be observed when examining the performance of the logistic regression model.  Overall, the model performed exceptionally well with a 99% accuracy rate. The model excelled at identifying healthy loans, scoring a 100% success rate in precision and recall.  The model did drop off slightly when identifying high-risk loans, scoring 87% in precision and 89% in recall.  One potential reason for the drop off in the high-risk loans results may be due to the small sample size provided for the model, as it only accounted for 3.2% of the total data examined.  Increasing this sample size may provide greater learning opportunities for the model, thus boosting its performance.  It may also be prudent to The data was read into a Pandas DataFrame for analysis.  
<br>
<img src="ReadMe Pics/Pic 1.png" width="858" height="167">

<br>


The “loan_status” column was removed from the DateFrame and it was placed in its own DataFrame resulting in two standalone DataFrames of data.  The two Dataframes can be viewed below. 

<br>
<img src="ReadMe Pics/Pic 3.png" width="785" height="155">
<img src="ReadMe Pics/Pic 2.png" width="299" height="136">

expose this data to other machine learning models to see if the change affects the performance results.           

In this challenge, we utilized a structured machine learning logistic regression model to evaluate the loan risk of borrowers.  This determination was based off a variety of factors.  These factors include: <br>
* Loan Size
* Interest Rate
* Borrower Income
* Debt to Income Ratio
* Number of Revolving Accounts
* Past Negative Credit Marks
* Total Debt
The confusion matrix results show:
<br>
* 18,679 individuals were CORRECTLY identified as credit worthy (True Negative)
* 558 individuals were CORRECTLY identified as not credit worthy (True Positive)
* 67 individuals that were INCORRECTLY identified as not credit worthy (False Negative)
* 80 individuals were INCORRECTLY identified as credit worthy (False Positive)

The rows and columns were summed and compared to assess accuracy and precision.  Both aggregate totals were 19,384 so we can consider the model to be accurate and precise.

<img src="ReadMe Pics/Pic 17.png" width="421" height="287">

The classification report results show:
<br>
* The accuracy of the entire model was 99%
* The precision for healthy loans was 100% 
* The recall for healthy loans was 100%
* The precision for high-risk loans was 87% 
* The recall for high-risk loans was 89%  
