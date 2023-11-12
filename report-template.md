# Alphabet Soup Charity Report

Analysis Overview:
Alphabet Soup, a nonprofit foundation, is in need of a predictive tool to assess the success of funding applicants. The dataset comprises information on over 34,000 organizations funded by Alphabet Soup, including various metadata columns. The objective is to construct a binary classifier using machine learning and neural networks.

Steps Taken:
Imported Dependencies:

Brought in essential libraries, including sklearn, Pandas, and TensorFlow.
Data Loading and Preprocessing:

Loaded the 'charity_data.csv' dataset into a Pandas dataframe.
Eliminated unnecessary columns ('EIN' and 'NAME').
Applied binning for infrequent categorical variables in 'CLASSIFICATION' and 'APPLICATION_TYPE' columns.
Converted categorical data into numeric format using pd.get_dummies.
Separated the preprocessed data into features and target arrays.
Divided the data into training and testing datasets.
Neural Network Model Building:

Compiled, trained, and assessed the model.
Endeavored to optimize the model using the keras-tuner library.
Results:
Neural Network Attempt 1:
Activation: "relu", "relu", "relu"
Hidden Nodes Layer 1: 9, Layer 2: 18
Accuracy: 73%
Loss: 0.55
Neural Network Attempt 2:
Activation: "relu", "relu", "relu"
Hidden Nodes Layer 1: 9, Layer 2: 18, Layer 3: 25
Accuracy: 73%
Loss: 0.56
Neural Network Attempt 3:
Activation: "relu", "tanh", "tanh"
Hidden Nodes Layer 1: 9, Layer 2: 18, Layer 3: 29
Accuracy: 73%
Loss: 0.55
Summary:
Despite experimenting with various layer configurations and activation functions, the model fell short of achieving the targeted 75% accuracy. Further adjustments and refinements may be necessary, such as exploring different architectures, fine-tuning hyperparameters, and addressing potential issues like overfitting. Additionally, a comprehensive evaluation of the data's nature and potential feature engineering could contribute to enhancing the model's performance.


