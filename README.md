# Empowering-IoT-Cybersecurity-Network-Attacks-with-Machine-Learning



## Description

This project leverages machine learning techniques to classify network attacks such as Port Scanning, Denial of Service (DoS), and malware. The input data is in the Netflow V9 format, which is a standard format used by Cisco.

The classification is performed using the following models:

- K-Nearest Neighbors (KNN)
- Support Vector Machine Classifier (SVC) with RBF (Radial Basis Function) kernel
- Pipeline with Principal Component Analysis (PCA) and Support Vector Machine Classifier (SVC)
- Bagging Classifier (based on SVC with RBF kernel)
- Random Forest Classifier
- Extra Trees Classifier
- Neural Network (MLPClassifier)

The project is implemented in Python using Jupyter Notebook and several popular libraries, including [UMAP](https://umap-learn.readthedocs.io/), [Pandas](https://pandas.pydata.org), [NumPy](https://numpy.org), [Scikit-Learn](https://scikit-learn.org/), [Matplotlib](https://matplotlib.org), and [Seaborn](https://seaborn.pydata.org).


## Datasets

The dataset used for this project is in the NetFlow V9 format (documented by Cisco, available [here](https://www.cisco.com/en/US/technologies/tk648/tk362/technologies_white_paper09186a00800a3db9.html)). It consists of two files: train_net.csv and test_net.csv.

The train_net.csv file provides information on when a particular alert is likely to occur, while the test_net.csv file is used solely for testing purposes and does not contain a target variable for evaluating model performance.

The dataset is quite large:

- `train_net.csv`: approximately 4 million packets (from 14'066 unique network hosts)
- `test_net.csv`: approximately 2 million packets (from 6'186 unique network hosts)



### Dataset authors

Maria-Elena Mihailescu, Darius Mihai, Mihai Carabas, Mikolaj Komisarek, Marek Pawlicki, Witold Holubowicz, Rafal Kozik:
The Proposition and Evaluation of the RoEduNet-SIMARGL2021 Network Intrusion Detection Dataset. Sensors 21(13): 4319 (2021)

[Kaggle link](https://www.kaggle.com/datasets/ashtcoder/network-data-schema-in-the-netflow-v9-format)
