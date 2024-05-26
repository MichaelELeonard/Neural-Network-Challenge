# Week 21 Challenge – Deep-Learning

<img src="ReadMe Pics/Cover 3.png" width="745" height="305">


# Background
The nonprofit foundation Alphabet Soup wants a tool that can help it select the applicants for funding with the best chance of success in their ventures.  A CSV was received From Alphabet Soup’s business team, containing more than 34,000 organizations that have received funding from Alphabet Soup over the years. Use machine learning and neural networks, create a binary classifier that can predict whether applicants will be successful if funded by Alphabet Soup.



# Preprocessing
<br>
For the preprocessing of the data, the data was initially read into a Pandas DataFrame and the EIN and NAME columns were removed.  The variable IS_SUCCESSFUL is identified to be the ‘target’ of the model with the ‘feature’ variables to include: 
<br>
<br>

* Application Type
* Affiliation
* Classification
* Use Case
* Organization
* Status
* Income Amt
* Special Considerations
* Ask Amount

### Import and read the charity_data.csv
<img src="ReadMe Pics/Pic 1.png" width="1602" height="209">

### Drop the non-beneficial ID columns, 'EIN' and 'NAME'
<img src="ReadMe Pics/Pic 2.png" width="1195" height="212">

### Binning the Data
Cut off values for binning ‘APPLICATION_TYPE’ (500) and  ‘CLASSIFICATION’ (1800) were established with any data below these thresholds placed in category ‘Other’

<img src="ReadMe Pics/Pic 4.png" width="215" height="217">




### The data was converted to numeric data with pd.get_dummies
<img src="ReadMe Pics/Pic 5.png" width="1733" height="240">

Finally, the data was split and was placed in features and target arrays, an instance for the StandardScaler was established, fit to the data, and the data was scaled. 
<br>

# Compile, Train and Evaluate the Model
A Deep Learning - Neural Network model was established, compiled, fit, and trained.   The model was run for 200 epochs.  Model characteristics included:   
* Two hidden layers <br>
** Hidden layer one – 8 neurons, activation function ‘relu’<br>
** Hidden layer two – 5 neurons, activation function ‘relu’<br>
* Output layer – 1 neuron, activation function ‘sigmoid’<br>  

<img src="ReadMe Pics/Pic 6.png" width="539" height="291">

# The Results
The model produced a 73.17 predictive accuracy and a loss of .055
<img src="ReadMe Pics/Pic 7.png" width="589" height="59">
<img src="ReadMe Pics/Accuracy working.png" width="598" height="437">

# Optimization Models
### Overview
Alphabet Soup wants a tool that can help it select the applicants for funding with the best chance of success in their ventures.  Use machine learning and neural networks, create a binary classifier that can predict whether applicants will be successful if funded by Alphabet Soup.  Five optimization model permutations were constructed in an attempt to boost the model’s accuracy above 75%.   For all five optimization models the   

### Targets and Features
The variable ‘Is Successful‘ was identified to be the ‘target’ for all five of the models with the ‘feature’ variables to include: 
<br>
<br>

* Application Type
* Affiliation
* Classification
* Use Case
* Organization
* Status
* Income Amt
* Special Considerations
* Ask Amount

### Removed Columns
The 'EIN' and 'Name' columns were removed from the dataset and they were not needed for the model.



<img src="ReadMe Pics/Cover 4.png" width="799" height="469"> 
