# Experimental Evaluation of SVM Kernels for Binary Image Classification

George Ioannidis, undergraduate student, ECE AUTH

## Overview

This project focuses on binary image classification using Support Vector Machines, an MLP model and classical baseline classifiers. The original CIFAR-10 dataset is transformed into a binary classification problem by grouping the classes into two categories: Animals and Vehicles.

The goal is to compare the testing performance of different SVM kernels with simpler baseline methods and a neural network trained with Hinge Loss.

## Methods

The SVM models include:

* Linear Kernel SVM
* RBF Kernel SVM
* Polynomial Kernel SVM

The additional comparison models include:

* Multi-Layer Perceptron with Hinge Loss
* Nearest Centroid
* 1-Nearest Neighbor
* 3-Nearest Neighbor

For the SVM experiments, different hyperparameters were evaluated using:

* Grid Search
* 5-Fold Cross-Validation
* different values of C
* different gamma values
* different polynomial degrees

## Results

The best-performing model was the RBF SVM, achieving 90.27% test accuracy on the binary Animals vs Vehicles classification task.

The final comparison showed that non-linear SVM kernels performed better than the Linear SVM and the baseline classifiers. The MLP with Hinge Loss also achieved competitive performance.

## Files

* `code/svm_kernel_evaluation.ipynb`: SVM kernel experiments and hyperparameter tuning
* `code/mlp_hinge_baselines.ipynb`: MLP with Hinge Loss and baseline classifiers
* `Report.pdf`: project report
