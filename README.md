<img src="ReadMe Pics/Cover 3.png" width="745" height="305">

# Neural Network Challenge

Neural Network Code - https://github.com/MichaelELeonard/deep-learning-challenge/blob/main/AlphabetSoupCharity_Working.ipynb
<br>

Optimization #1 - https://github.com/MichaelELeonard/deep-learning-challenge/blob/main/AlphabetSoupCharity_Optimization_%231.ipynb
<br>

Optimization #2 - https://github.com/MichaelELeonard/deep-learning-challenge/blob/main/AlphabetSoupCharity_Optimization_%232.ipynb
<br>

Optimization #3 - https://github.com/MichaelELeonard/deep-learning-challenge/blob/main/AlphabetSoupCharity_Optimization_%233.ipynb

# Background
The nonprofit foundation Alphabet Soup wants a tool that can help it select the applicants for funding with the best chance of success in their ventures.  A CSV was received from the Alphabet Soup’s business team, containing more than 34,000 organizations that have received funding from Alphabet Soup over the years. The goal is to utilize machine learning and neural networks to create a binary classifier that can predict whether applicants will be successful if funded by Alphabet Soup.
<br>

# Preprocessing
The data was read into a Pandas DataFrame and the EIN and NAME columns were removed.  The variable ‘Is Successful’ was identified to be the ‘target’ of the model with the ‘feature’ variables to include: 
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
<img src="ReadMe Pics/Pic 1.png" width="1602" height="180">

### Drop the non-beneficial ID columns, 'EIN' and 'NAME'
<img src="ReadMe Pics/Pic 2.png" width="1195" height="212">

### Binning the Data
Cut off values were established for binning ‘Application Type” (500) and  ‘Classification’ (1800), with any data below these thresholds placed in category ‘Other’

<img src="ReadMe Pics/Pic 4.png" width="215" height="217">




### The data was converted to numeric data with pd.get_dummies
<img src="ReadMe Pics/Pic 5.png" width="1733" height="215">

Finally, the data was split and was placed in features and target arrays, an instance for the StandardScaler was established, fit to the data, and the data was scaled. 
<br>
<br>

# Compile, Train and Evaluate the Model
A Deep Learning - Neural Network model was established, compiled, fit, and trained.   The model was run for 200 epochs, with model characteristics including:   
* Two hidden layers <br>
* Hidden layer one – 8 neurons, activation function ‘relu’<br>
* Hidden layer two – 5 neurons, activation function ‘relu’<br>
* Output layer – 1 neuron, activation function ‘sigmoid’<br>  

<img src="ReadMe Pics/Pic 6.png" width="539" height="291">

# The Results
The model produced a 73.17% predictive accuracy rate and a loss of 0.55

<br>
<img src="ReadMe Pics/Pic 7.png" width="589" height="59">
<img src="ReadMe Pics/Accuracy working.png" width="598" height="437">

# Optimization Modeling and Results
## Overview
Alphabet Soup wants a tool that can help it select the applicants for funding with the best chance of success in their ventures.  Use machine learning and neural networks, create a binary classifier that can predict whether applicants will be successful if funded by Alphabet Soup.  Three optimization model permutations were constructed in an attempt to boost the model’s accuracy above 75%.   

## Targets and Features
The variable ‘Is Successful‘ was identified to be the ‘target’ for all three of the models and the ‘feature’ variables included: 
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

## Removed Columns
The 'EIN' and 'Name' columns were removed from the dataset, and they were not needed for the model.  ‘Application Type’ (500) and ‘Classification’ (1800) were binned to remove any extraneous data from the dataset.  
<br>


## Compiling, Training, and Evaluating the Optimization Models
An outline of the optimization techniques used for each optimization model and their respective results are as follows:
### Optimization Model #1
Optimization #1 - https://github.com/MichaelELeonard/deep-learning-challenge/blob/main/AlphabetSoupCharity_Optimization_%231.ipynb

* Three hidden layers <br>
* Hidden layer one – 15 neurons, activation function ‘relu’<br>
* Hidden layer two – 15 neurons, activation function ‘relu’<br>
* Hidden layer three – 15 neurons, activation function ‘relu’<br>
* Output layer – 1 neuron, activation function ‘sigmoid’<br>  
This attempt was designed to boost the complexity of the  optimization model by creating 3 hidden layers with 15 neurons per layer to assess if the accuracy results would increase.  Unfortunately, the results came in less than the original attempt, producing 72.8% predictive accuracy and a loss of 0.55
<img src="ReadMe Pics/Opp Output Pic1.png" width="525" height="289">
<img src="ReadMe Pics/Opp Output Pic2.png" width="587" height="62">
<img src="ReadMe Pics/Opp Output Pic3.png" width="589" height="435">


### Optimization Model #2
Optimization #2 - https://github.com/MichaelELeonard/deep-learning-challenge/blob/main/AlphabetSoupCharity_Optimization_%232.ipynb

* Four hidden layers <br>
* Hidden layer one – 20 neurons, activation function ‘LeakyReLU’<br>
* Hidden layer two – 20 neurons, activation function ‘LeakyReLU’<br>
* Hidden layer three – 20 neurons, activation function ‘relu’<br>
* Hidden layer four – 20 neurons, activation function ‘relu’<br>
* Output layer – 1 neuron, activation function ‘sigmoid’<br>  
The complexity of this optimization model was again increased by creating 4 hidden layers with 20 neurons per layer in an attempt to boost model’s performance.  ‘LeakyReLU” was used as the activation function for the first two hidden layers and the ‘Classification’ bin cutoff value was reduced to 280 to try and bring more variability to the model.  Unfortunately, the results again came in at less than the original attempt, producing 72.7% predictive accuracy and a loss of 0.56

<img src="ReadMe Pics/Opp Output Pic4.png" width="522" height="316">
<img src="ReadMe Pics/Opp Output Pic5.png" width="596" height="52">
<img src="ReadMe Pics/Opp Output Pic6.png" width="633" height="436">


### Optimization Model #3
Optimization #3 - https://github.com/MichaelELeonard/deep-learning-challenge/blob/main/AlphabetSoupCharity_Optimization_%233.ipynb

* Six hidden layers <br>
* Hidden layer one – 30 neurons, activation function ‘LeakyReLU’<br>
* Hidden layer two – 30 neurons, activation function ‘relu’<br>
* Hidden layer three – 30 neurons, activation function ‘LeakyReLU’<br>
* Hidden layer four – 30 neurons, activation function ‘relu’<br>
* Hidden layer five – 30 neurons, activation function ‘LeakyReLU’<br>
* Hidden layer six – 30 neurons, activation function ‘relu’<br>
* Output layer – 1 neuron, activation function ‘sigmoid’<br>  
The complexity of this optimization model was again increased by creating 6 hidden layers with 30 neurons per layer to see if the accuracy results would increase.  Epochs were increased to 400 and ‘LeakyReLU’ was used as the activation function for layers one, three and five, with ‘ReLU’ used for layers two, four and six.  Finally, the ‘Classification’ bin cutoff value was reduced to 280 to try and bring more variability to the model.  The results again stubbornly came in less than the original attempt, producing 72.8% predictive accuracy and a loss of 0.59

<img src="ReadMe Pics/Opp Output Pic7.png" width="520" height="382">
<img src="ReadMe Pics/Opp Output Pic8.png" width="577" height="61">
<img src="ReadMe Pics/Opp Output Pic9.png" width="577" height="438">

## Optimization Summary
With the three optimization models we were attempting to boost the model’s accuracy performance by using a variety of model optimization techniques.  The model optimization techniques implemented included:
* Adding more neurons
* Adding more hidden layers
* Changing activation functions
* Adding more epochs.  

<br>
Unfortunately, none of the optimization techniques was able to produce the desired goal of achieving a 75% accuracy percentage for the model.  Future steps to achieve the 75% accuracy percentage could include:
<br>
<br>

* Trying different model structures including Decision Trees, Randon Forrest and Supervised and Unsupervised learning
* Implement Tensorflow 2.0 within our model to automate our neural network model optimization

<br>
<img src="ReadMe Pics/Cover 4.png" width="799" height="469">
