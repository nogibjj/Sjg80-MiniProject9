# Sjg80-MiniProject9
Cloud-Hosted Notebook Data Manipulation

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/shailajgg/Git-Class-Fall-2023/blob/main/Cloud_hosted_notebook.ipynb)

# Data Manipulation and Analysis using Google Colab

This repository contains code and data for manipulating and analyzing a dataset using Google Colab, a cloud-based Jupyter notebook environment. In this README, we will explain how the data manipulation was performed and provide information on how to access the hosted notebook on Google Colab.

## Dataset

The dataset used in this project is the Iris dataset, which is included in the scikit-learn library. The Iris dataset is a popular dataset in machine learning and consists of four features (sepal length, sepal width, petal length, and petal width) for three different species of iris flowers (setosa, versicolor, and virginica). The objective of this project is to classify the species of iris flowers based on these features.

## Data Manipulation

The data manipulation process involves the following steps:

1. **Loading the Dataset:** We start by importing the Iris dataset from scikit-learn using the following code:

   ```python
   from sklearn.datasets import load_iris
   iris = load_iris()
   ```

2. **Data Summary:** We extract some statistics from the dataset using Pandas. Summary statistics, feature names, and target names are displayed to understand the data:

   ```python
   df = pd.DataFrame(data=iris.data, columns=iris.feature_names)
   summary_stats = df.describe()
   feature_names = iris.feature_names
   target_names = iris.target_names
   ```

![descarga](https://github.com/nogibjj/Sjg80-MiniProject9/assets/142270941/0e87c370-a332-4553-be19-0ac2d670243d)

3. **Data Visualization:** We create scatterplots to visualize the relationships between different features and target species to gain insights into the data.

![descarga (1)](https://github.com/nogibjj/Sjg80-MiniProject9/assets/142270941/9bd0dcfd-5f80-4895-9803-6603f3b7df29)


4. **Data Preprocessing:** Data preprocessing steps include splitting the dataset into training and testing sets and standardizing the features using StandardScaler.

![descarga (4)](https://github.com/nogibjj/Sjg80-MiniProject9/assets/142270941/e6af2d4a-fd90-4c46-9709-4dbbaf12d83a)

5. **Model Building:** We use a Support Vector Classifier (SVC) model for classification. We perform hyperparameter tuning using GridSearchCV to optimize the model's performance.


6. **Evaluation:** The model's performance is evaluated using a confusion matrix to visualize classification results and a scoring metric.

![descarga (2)](https://github.com/nogibjj/Sjg80-MiniProject9/assets/142270941/94c34bf7-acaf-43cd-aa15-544453fef4b6)

## Access the Notebook on Google Colab

To access the complete notebook with the code and detailed explanations, you can use the following link to the hosted Google Colab notebook:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/shailajgg/Git-Class-Fall-2023/blob/main/Cloud_hosted_notebook.ipynb)

Simply click on the link, and it will open the notebook in your web browser. You can run the code cells and explore the data manipulation and analysis process in more detail.


