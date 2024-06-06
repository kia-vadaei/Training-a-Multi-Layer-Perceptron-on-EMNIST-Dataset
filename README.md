# Training a Multi Layer Perceptron on `EMNIST` Dataset

## Author
- **Kianoosh Vadaei**: Researcher

### Contact Information
- Kianoosh Vadaei: [Email](mailto:kia.vadaei@gmail.com), [LinkedIn](https://www.linkedin.com/in/kianoosh-vadaei-0aa58611b/), [GitHub](https://github.com/kia-vadaei)

## Introduction
This repository provides an implementation of a **Multi-Layer Perceptron (MLP) for EMNIST Classification**. The steps covered include:
1. Data Loading
2. Data Preprocessing
3. Model Building
4. Model Training
5. Model Evaluation
6. Conclusion

## Table of Contents
1. [Introduction](#introduction)
2. [Data Loading](#data-loading)
3. [Data Preprocessing](#data-preprocessing)
4. [Model Building](#model-building)
5. [Model Training](#model-training)
6. [Model Evaluation](#model-evaluation)
7. [Conclusion](#conclusion)

## Data Loading
In this section, we load the dataset, which creates two sets: training and testing datasets. The data split mode is balanced, resulting in `47` classes, with some classes removed.

## Data Preprocessing
We preprocess the data by transforming it to tensors, normalizing it, and creating train loaders and data batches. We also display the size of each picture in each batch.

## Model Building
We build and train an MLP model to classify the labels from the training data. This model has `4` hidden layers, an input size of `784` (28x28), and an output size of `47` classes.

## Model Training
The model is trained with the training data using a scheduled learning rate and L2 regularization for 100 epochs until convergence. If the `show_plot` parameter is set to `True` (default), a plot showing the reduction in training loss and testing loss is displayed.

## Model Evaluation
The model's performance is evaluated using various metrics. The test report of classification metrics includes:

- **Accuracy**: `xx.xx %`
- **Precision**: `xx.xx %`
- **Recall**: `xx.xx %`
- **F1 Score**: `xx.xx %`

