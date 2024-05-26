# Week 21 Challenge – Deep-Learning

<img src="ReadMe Pics/Cover 3.png" width="745" height="305">


# Background
The nonprofit foundation Alphabet Soup wants a tool that can help it select the applicants for funding with the best chance of success in their ventures.  A CSV was received From Alphabet Soup’s business team, containing more than 34,000 organizations that have received funding from Alphabet Soup over the years. Use machine learning and neural networks, create a binary classifier that can predict whether applicants will be successful if funded by Alphabet Soup.



# Preprocessing
<br>
For the preprocessing of the data, the data was initially read into a Pandas DataFrame and the EIN and NAME columns were removed.  

### Import and read the charity_data.csv

<img src="ReadMe Pics/Pic 1.png" width="1602" height="209">


### Drop the non-beneficial ID columns, 'EIN' and 'NAME'

<img src="ReadMe Pics/Pic 2.png" width="1195" height="212">


### Determine the number of unique values in each column

<img src="ReadMe Pics/Pic 3.png" width="277" height="204">


### Look at APPLICATION_TYPE value counts to identify and replace with "Other"
### Choose a cutoff value and create a list of application types to be replaced use the variable name `application_types_to_replace`
### Choose a cutoff value and create a list of classifications to be replaced use the variable name `classifications_to_replace`
### Convert categorical data to numeric with `pd.get_dummies`
### Split our preprocessed data into our features and target arrays
### Create a StandardScaler instances
### Fit the StandardScaler
### Scale the data

# Compile, Train and Evaluate the Model
## Define the model - deep neural net, i.e., the number of input features and hidden nodes for each layer.
## Compile the model
## Train the model
## Evaluate the model using the test data
## Export our model to HDF5 file

### Summary






<img src="ReadMe Pics/Pic 4.png" width="215" height="217">
<img src="ReadMe Pics/Pic 5.png" width="1733" height="240">
<img src="ReadMe Pics/Pic 6.png" width="539" height="291">
<img src="ReadMe Pics/Pic 7.png" width="589" height="59">
<img src="ReadMe Pics/Cover 1.png" width="760" height="550">
<img src="ReadMe Pics/Cover 2.png" width="846" height="327">

<img src="ReadMe Pics/Cover 4.png" width="799" height="469">
<img src="ReadMe Pics/Cover 5.png" width="798" height="421">



The classification report results show:
<br>
* The accuracy of the entire model was 99%
* The precision for healthy loans was 100% 
* The recall for healthy loans was 100%
* The precision for high-risk loans was 87% 
* The recall for high-risk loans was 89%  
