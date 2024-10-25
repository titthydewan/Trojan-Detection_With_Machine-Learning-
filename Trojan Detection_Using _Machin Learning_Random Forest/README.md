# Trojan-Detection-in-Machine-Learning-Using-Random-Forest

**Overview**

This project aims to classify Trojan malware samples as either "Trojan Infected" or "Trojan Free" using a dataset. The methodology involves a series of data preprocessing steps, feature engineering, model training, and evaluation. Specifically, it employs Random Forest and Decision Trees to achieve this classification task and assesses model performance through various metrics.


**Table of Contents**

1.Dataset

2.Data Preprocessing

3.Feature Engineering

4.Model Training and Evaluation

5.Combining Decision Trees

6.Final Model and Results

7.Classification Report

8.F-Score Calculation

9.Dependencies


**Dataset**

The dataset used for this project is trojantrojannew.csv, which includes a set of features related to Trojan malware samples along with a label indicating whether a sample is "Trojan Infected" or "Trojan Free."

**Data Preprocessing**

1.Loading the Data:

The dataset is loaded into a DataFrame.

![image](https://github.com/Poushali-dev/Trojan-Detection-in-Machine-Learning-Using-Random-Forest/assets/175179861/76b0b1a2-1de7-46a8-b3c3-376c11abda9e)

2.Creating Dummy Variables:

Convert the categorical Label column into dummy/indicator variables.

![image](https://github.com/Poushali-dev/Trojan-Detection-in-Machine-Learning-Using-Random-Forest/assets/175179861/b288972e-de0a-4268-8b9c-5e343a55c557)

3.Updating the DataFrame:

Add dummy variables to the DataFrame and remove the original Label column and the redundant Trojan Free column.

![image](https://github.com/Poushali-dev/Trojan-Detection-in-Machine-Learning-Using-Random-Forest/assets/175179861/863816ae-b96d-4fa1-8c38-27a30b0846fe)

4. Preparing Feature and Target Variables:
   
Define features (X) and target variable (Y), and drop the 'Circuits' column.

![image](https://github.com/Poushali-dev/Trojan-Detection-in-Machine-Learning-Using-Random-Forest/assets/175179861/fabf8de2-ef10-47c6-b21a-9ccbb5bb1d29)


**Feature Engineering**

1. Generate Unique Feature Combinations:
   
Create 70 unique combinations of features, each containing 4 features.

![image](https://github.com/Poushali-dev/Trojan-Detection-in-Machine-Learning-Using-Random-Forest/assets/175179861/89563456-dcdc-42e5-afeb-1dfbd25f464c)


**Combining Decision Trees**

1. Training Decision Trees:
   
Train 70 Decision Trees, evaluate each model, and calculate performance metrics.

![image](https://github.com/Poushali-dev/Trojan-Detection-in-Machine-Learning-Using-Random-Forest/assets/175179861/b4ec46c8-1192-4705-a34c-8e84725ef0fe)

2. Selecting the Best Models:
   
Find the best decision trees based on accuracy and specific intervals.

![image](https://github.com/Poushali-dev/Trojan-Detection-in-Machine-Learning-Using-Random-Forest/assets/175179861/19f56b92-3618-43b5-a3e6-1f9379259742)


**Final Model and Results**
1. Training Final Random Forests:
   
Train final Random Forest models based on the best decision trees.

![image](https://github.com/Poushali-dev/Trojan-Detection-in-Machine-Learning-Using-Random-Forest/assets/175179861/2958b67d-da2e-466a-a011-45467b436f57)

2. Evaluating Final Model:
   
Evaluate the final model's performance and generate the classification report.

![image](https://github.com/Poushali-dev/Trojan-Detection-in-Machine-Learning-Using-Random-Forest/assets/175179861/f9939e19-4b85-474e-b487-64a9784f8985)

3. Classification Report
   
The classification report provides the counts for True Positives (TP), False Positives (FP), True Negatives (TN), and False Negatives (FN), along with the calculation of the F-Score.

![image](https://github.com/Poushali-dev/Trojan-Detection-in-Machine-Learning-Using-Random-Forest/assets/175179861/e5ac9690-3dc0-435e-8e4a-0395d77f1956)

**Dependencies**

To run this project, you will need the following Python packages:

pandas

numpy

scikit-learn

You can install them using pip:

**pip install pandas numpy scikit-learn**











