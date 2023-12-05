<img src="site-logo.svg" width=250>

# Kaggle Playground Competition: Regression with a Mohs Hardness Dataset

## Overview

This repository contains my experiments and submissions for the Kaggle Playground competition. The goal of this competition is to explore and test different dense network architectures on the provided training and testing datasets. The competition provides a unique opportunity to experiment with various deep learning models and techniques.

## Dataset

The dataset for this competition (both train and test) was generated from a deep learning model trained on the Prediction of Mohs Hardness with Machine Learning dataset. Feature distributions are close to, but not exactly the same, as the original. Feel free to use the original dataset as part of this competition, both to explore differences as well as to see whether incorporating the original in training improves model performanc

The dataset (train.csv) is loaded into a Pandas DataFrame to understand its structure and contents using:

    filepath = "/kaggle/input/playground-series-s3e25/train.csv"
    dataset = pd.read_csv(filepath)
    dataset.info()

### Preparation

The target variable, 'Hardness,' is separated from the input features. The dataset is then normalized to ensure consistent scales for training.

    test_dataset = pd.read_csv("/kaggle/input/playground-series-s3e25/test.csv")

    # Normalizing test dataset
    for column in test_dataset:
        if column != 'id':
            test_dataset[column] = test_dataset[column] / max(test_dataset[column])

    # Making predictions
    predictions = model.predict(test_dataset)

## Experimentation

I've implemented and tested several neural network architectures to find the most effective model for the given task. Each experiment is organized into its own Jupyter Notebook for clarity. The following architectures have been explored:

1. **DNN Model 1: Basic Dense Layers**
    - Architecture: 

    <img src="Arch\DNN model arch.png" width=300>

    - Results: Performed 2nd best, best score = 1.0035

2. **DNN Model 2: Skip connections**
    - Architecture: 

    <img src="Arch\DNN skip connection model arch.png" width=200>

    - Results: Performed worst, best score = 1.0022

3. **RNN Model: LSTM layers**
    - Architecture: 
    
    <img src="Arch\RNN model arch.png" width=200>
    
    - Results: Performed best, best score = 0.7128

## Submission

The best-performing model will be submitted to the Kaggle competition for evaluation. Results and leaderboard rankings will be updated accordingly.



## Acknowledgments

- This work is inspired by the Kaggle community and the valuable insights shared by fellow participants.
- Special thanks to Kaggle for hosting this playground competition and providing an opportunity for experimentation.

## License

This project is licensed under the [MIT License](LICENSE).
