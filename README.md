## Introduction

The fields of machine learning and artificial intelligence have made great strides in recent years, automating laborious, time-consuming, and manually implemented algorithms in favour of strong, dynamic language libraries, which have logic preprogrammed with simple language syntax and speed up implementation. Data mining techniques have recently undergone significant advancements that allow users to gain a deeper understanding of various datasets, infer better targeted predictions, and uncover a number of previously unknown or unobserved interpretations of the data.

Complicated datasets with a sizable size and subpar usability scores may point to a potential trend of mediocrity in the prediction accuracies for the model built using these datasets. It need not be a strict rule, though, and such generalised notions can be refuted using modern, sophisticated computing tools. The project uses a dataset with a similar description and investigates a number of techniques to develop appropriate prediction models using Classification Mining Techniques and Deep Learning concepts to produce predictions that are more accurate than those in the base paper without overfitting the model.

## Project Team

|Sl.No. | Name  |
|1|Arjun Rajesh Nair

## Project Objective

Jock A. Blackard and Denis J. Dean used discriminant analysis and an artificial neural network in 1999 to predict the forest cover in different parts of the Roosevelt National Forest in Colorado, USA.

But according to his paper, the model they built using artificial neural networks on various columns of data only had a 71.1% prediction accuracy. Although this approach was superior to the previously used traditional Discriminant Analysis, our goal in this project is to develop a variety of classification models in order to improve accuracy while still using the same dataset.

This dataset contains data on the kind of tree, the amount of shadows, the surrounding wildness, the distance to nearby landmarks (roads, for example), the type of soil, the terrain of the area, etc. There are more than 0.5 million item sets in the dataset, making it very big. According to prestigious data science websites, its usability is 5.9.

The source for the dataset used above, [Covertype] (https://archive.ics.uci.edu/ml/datasets/Covertype), can be found here. The dataset is also available in the main branch of the repository as [covtype.csv] (https://github.com/Arjun-R-Nair/Forest-cover-prediction/blob/main/covtype.csv). Lastly, the model's performance in terms of accuracy and total prediction performance is evaluated for effectiveness.

## Tools Used

To achieve the project objective I used the following tools -
* **Classification Mining Techniques**
  * Logistic Regression
  * Gaussian Naive Bayes'
  * K-Nearest Neighbors
  * Support-Vector Machine
  * Random Forest Classification

* **Deep Learning**
  * Artificial Neural Network

* **Python Language Libraries**
  * Seaborn
  * Matplotlib
  * Scikit-learn
  * Pandas
  * Keras
  * Tensorflow
 
* **R Language Libraries** 
  * Tidyverse
  * Skimr

## Methodology

1. Understanding the dataset's components.
2. Developing visualisations to help us comprehend and make it possible for us to choose the ideal mix of data columns for high accuracy.
3. Using different categorization mining methods to develop models that provide a certain level of prediction accuracy for a particular set of data columns.
4. Properly fitting models and determining if any models have been over- or under-fitted.
5. Finding the optimum train-test split by repeatedly iterating over certain column combinations and methods and saving the prediction percentage and split content in a separate binary file for later use.
6. Applying deep learning to the dataset to get accurate predictions.
7. Evaluate the effectiveness of every method and, using this dataset, propose the algorithm that performs the best.

## Implementation

A segment of the visualisation has used the R language and its libraries to help us understand the dataset better. The rest of the visualisation, classification and DL analysis has been implemented with the help of Python libraries.

### Understanding the Data

The dataset contains the following 13 columns:

One of the seven different forms of tree cover that may be found in a forest. The observations are coded 1 through 7 in the data that was downloaded for the project. For clarity, we gave them new names. The United States Forest Service's classification of the principal cover type for 30m x 30m areas is used as the basis for observations. Our response variable is this.
Four of the six wilderness areas in the Roosevelt National Forest were utilised in this dataset (wilderness Area). Originally, they were one-hot encoded in the dataset. While most machine learning techniques would automatically one-hot encode categorical variables for us, we present them in lengthy form for better visualisation.
- Soil Type: The dataset identified 40 different kinds of soil; further information about the types is available at https://www.kaggle.com/uciml/forest-cover-type-dataset. Soil Type was initially one-hot encoded, like Wilderness Area.
- Elevation: The observation's altitude above sea level in metres.
- Aspect: The observation's aspect measured in azimuth degrees.
- Slope: The slope in degrees at which the observation is made.
- Hillshade 9am: The quantity of hillshade during the summer solstice observation at 9:00. This number ranges from 0 to 225.
- Hillshade Noon: The quantity of hillshade during the summer solstice observation at noon. This number ranges from 0 to 225.
- Hillshade 3pm: The quantity of hillshade during the summer solstice observation at 15:00. This number ranges from 0 to 225.
- Vertical Distance to Hydrology: The vertical distance in metres to the closest water source. Distance below a water source is indicated by negative numbers.
- Horizontal Distance To Hydrology: The distance in metres from the closest water source.
- Horizontal Distance to Roadways: The distance in metres to the closest roadway.
- Horizontal Distance To Fire Points: Measures the distance in metres from the closest wildfire ignition site.