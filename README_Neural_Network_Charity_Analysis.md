# NEURAL NETWORK CHARITY ANALYSIS

## OVERVIEW

### The purpose of this analysis is to help the charitable foundation, Alphabet Soup, predict where to make investments.

### Using machine learning and neural networks we will use the features in the provided dataset to create a binary classifier that is capable of predicting whether charity applicants will be successful if funded by Alphabet Soup.

### The dataset is a csv file containing more than 34,000 organizations that have received funding from Alphabet Soup over the years.

### There will be 4 deliverables in this analysis:

### 1) Preprocessing Data for a neural network model

### 2) Compile, train and evaluate the model.

### 3) Optimize the model.

### 4) Provide a written report on the Neural Network Model.

## RESOURCES

### File: charity_data.csv

### sklearn.model_selection. (import train_test_split)

### sklearn.preprocessing.  (import StandardScaler, OneHotEncoder)

### pandas

### Tensorflow


## RESULTS

### Read Charity Data

![__](https://github.com/Johnnytoobadman/Neural_Network_Charity_Analysis/blob/main/Images/01.png)

### Drop EIN and Name

![__](https://github.com/Johnnytoobadman/Neural_Network_Charity_Analysis/blob/main/Images/02.png)

### Unique Values

![__](https://github.com/Johnnytoobadman/Neural_Network_Charity_Analysis/blob/main/Images/03.png)

### Counts for Binning

![__](https://github.com/Johnnytoobadman/Neural_Network_Charity_Analysis/blob/main/Images/04.png)

### Value Counts Plot

![__](https://github.com/Johnnytoobadman/Neural_Network_Charity_Analysis/blob/main/Images/04.png)

### Application Counts

![__](https://github.com/Johnnytoobadman/Neural_Network_Charity_Analysis/blob/main/Images/06.png)

### Application Value Counts

![__](https://github.com/Johnnytoobadman/Neural_Network_Charity_Analysis/blob/main/Images/07.png)

### Visualize Value Counts

![__](https://github.com/Johnnytoobadman/Neural_Network_Charity_Analysis/blob/main/Images/08.png)

### Classifications

![__](https://github.com/Johnnytoobadman/Neural_Network_Charity_Analysis/blob/main/Images/09.png)

### Categorizations

![__](https://github.com/Johnnytoobadman/Neural_Network_Charity_Analysis/blob/main/Images/10.png)

### Encoded DataFrames

![__](https://github.com/Johnnytoobadman/Neural_Network_Charity_Analysis/blob/main/Images/11.png)

### Train and Evaluate (note low accuracy)

![__](https://github.com/Johnnytoobadman/Neural_Network_Charity_Analysis/blob/main/Images/12.png)

### Optimized Model (note slightly improved accuracy)

![__](https://github.com/Johnnytoobadman/Neural_Network_Charity_Analysis/blob/main/Images/13.png)


## SUMMARY

### Data Preprocessing:

### 1) The variables which are the targets for the models is Application type, Affiliation, Classification, use-case, organization, income amounts and special considerations.

### 2) The features which are targets for the model is Application Categories/Types.

### 3) The EIN and Name were dropped as they were neither variables or features

### Compiling, training and Evaluation the Model:

### 1) I initially started with 2 layers: 80 neurons with the Sigmoid model and 20 neurons with the Relu model.

### 2) I selected the Sigmoid model for the first layer to try it since in class we almost always did the relu model first.  Then I did the relu model.

### 3) I was not able to achieve the 75% target using this strategy.

### 4) In optimization I went with 4 layers , the first 3 being Relu with 80, 20 and 10 neuron respectively.  The 4th layer was using the Sigmoid model with only 10 neurons.

### 5) I switched around Relu vs Sigmoiod and increased neurons.  I received slightly better results with fewer neurons.  The initial accuracy results was at 72%.  After optimization I was able to increase the accuracy to around 73%.

### Overall I would be inclined to try the Deep Forest Model to see if accuracy could be improved.  I must say that Neural Networks are very fascinating!!

