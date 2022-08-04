# DTSA5510_Unsupervised_Model_Final
Final project for DTSA5510 Unsupervised Algorithms for Machine Learning

KAGGLE NOTEBOOK FOUND HERE: https://www.kaggle.com/code/mattison/water-pump-classification

KAGGLE Pump Sensor Data page: https://www.kaggle.com/datasets/nphantawee/pump-sensor-data

--> Note that the data CSV file was too large to put on github. You can find it at the second link above for the dataset page.

Water Pump Classification 💧
*using unsupervised learning techniques*

Overview
The problem: In today's society we are bombarded with much data but often do not know how to use that information. This dataset was put on Kaggle so that smart minds could find patterns in the sensor data given by a local water pump. The proposal for this project is to use machine learning to detect patterns in the sensor data so that the pump owners will be better able to understand when a failure is about to occur.

We begin this project by exploring the data provided. This project will use two unsupervised learning techniques including PCA (for feature extraction and dimensionalty reduction) and KMeans clusters. Then, supervised ML models are used to compare to the unsupervised Kmeans model. Finally, an overview and summary is provided at the end of the notebook.

Note: each code cell has a brief explaination of what that cell does. Some code cells are hidden for easier readability in Kaggle notebooks but you can easily expand them to see the full code.

1. 🧐 Exploratory Data Analysis
Exploratory data analysis (EDA) is very important when it comes to working with data. In this project we look at all the data first instead of splitting into traing-test sets. Because this notebook is completed for a school project, we will be doing some data anaylsis not normally recommended. For example, looking at all the data before splitting it. The EDA section uses visualizations and performs very preliminary data preprocessing steps, such as deleting empty columns.

2. 🤓 Preprocessing
In the preprocessing step, we need to get the most useful parts of the data to feed to the machine learning model. First we will deal with missing data using forward propogation. Then we will use a common unsupervised learning technqiue call Principle Component Analysis (PCA) to reduce the number of sensors used in the next steps. PCA is a great tool for feature reduction.

3. 🦾 Modeling
Next, using KMeans clustering (an unsupervised ML model) we will try to determine where the failures are. Because Kmeans is unsupervised, we will use the best model recommendation for number of clusters. To compare our models later, we need to use some sort of performance testing such as accuracy, recall and/or precision. Since, in reality, we do know the labels of the data we can find the best labeling throught permutation. The cavet to this technique is if there are more clusters than given labels, our model may perform poorly according to accuracy, recall or precision. We will discuss this later in the notebook more.

4. 🤜🤛 Model Comparison
After creating a KMeans cluster model, we will build a supervised learning model which also uses clustering such as K-Nearest Neighbors (KNN). We chose to use two clustering models for practice however, other possible models will be discussed in the following section.

5. 👏 Conclusions and Future Suggestions
This section includes a brief overview of the project and what was accomplished throughout. We review the different models used and how they performed. For a well-rounded project, we will reflect upon what could have been done differently to have a better model performance as well as things we could have changed in general and what their impact may have been.
