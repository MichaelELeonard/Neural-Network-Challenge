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



<img src="ReadMe Pics/Pic 1.png" width="648" height="391">
<img src="ReadMe Pics/Pic 2.png" width="648" height="391">
<img src="ReadMe Pics/Pic 3.png" width="648" height="391">
<img src="ReadMe Pics/Pic 4.png" width="648" height="391">
<img src="ReadMe Pics/Pic 5.png" width="648" height="391">
<img src="ReadMe Pics/Pic 6.png" width="648" height="391">
<img src="ReadMe Pics/Pic 7.png" width="648" height="391">
<img src="ReadMe Pics/Cover 1.png" width="648" height="391">
<img src="ReadMe Pics/Cover 2.png" width="648" height="391">
<img src="ReadMe Pics/Cover 3.png" width="648" height="391">
<img src="ReadMe Pics/Cover 4.png" width="648" height="391">
<img src="ReadMe Pics/Cover 5.png" width="648" height="391">



The classification report results show:
<br>
* The accuracy of the entire model was 99%
* The precision for healthy loans was 100% 
* The recall for healthy loans was 100%
* The precision for high-risk loans was 87% 
* The recall for high-risk loans was 89%  
