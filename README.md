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

## Conclusion
As observed, the 4-layer model provides the best accuracy. This is because the 4-layer model can better understand the complexities of the data and produce more accurate outputs. If we examine these models more closely, we see that the rate of cost reduction is also faster in the 4-layer model. This is evident as the model quickly comprehends major differences and similarities in the initial epochs and rapidly reduces cost or error.

One disadvantage of the 4-layer model is that its training time is significantly longer, requiring more computational resources or time for training. The report indicates that training this model takes approximately 28 minutes, which is twice the time needed for 2-layer and 3-layer models and 1.5 times the time required for a 4-layer model with a Sigmoid activation function.

I also trained the data with a 5-layer model, but the accuracy did not change significantly. Due to computational constraints, I am unable to train that model again.

To achieve higher accuracy, we can use a CNN model instead of an MLP model, as it extracts features more efficiently. However, there are other methods to increase the MLP model's accuracy, which I will briefly mention. These include using feature extraction methods like Hough and HOG from images, employing statistical criteria like Mutual Information or CHI2 for feature selection, and using dimension reduction techniques like PCA and LDA to reduce computational load. Their efficiency should be tested on the model.

Due to the course's focus not being on these pre-processing steps, I concentrated on the model itself and avoided implementing these methods.

Finally, we can save the obtained model and use it on different platforms.


Feel free to contact me via [email](mailto:kia.vadaei@gmail.com) or connect on [LinkedIn](https://www.linkedin.com/in/kianoosh-vadaei-0aa58611b/) or [GitHub](https://github.com/kia-vadaei) for any queries or discussions.
