<img src="site-logo.svg" width=250>

# Kaggle Playground Competition: Regression with a Mohs Hardness Dataset

## Overview

This repository contains my experiments and submissions for the Kaggle Playground competition. The goal of this competition is to explore and test different dense neural network architectures on the provided training and testing datasets. The competition provides a unique opportunity to experiment with various deep learning models and techniques.

## Dataset

The dataset for this competition (both train and test) was generated from a deep learning model trained on the Prediction of Mohs Hardness with Machine Learning dataset. Feature distributions are close to, but not exactly the same, as the original. Feel free to use the original dataset as part of this competition, both to explore differences as well as to see whether incorporating the original in training improves model performanc

- The dataset consists of [describe the dataset and its features].
- Training data: Hardness is the continuous target
- Testing data: the test dataset; your objective is to predict the value of Hardness
- Submission: a sample submission file in the correct format

## Experimentation

I've implemented and tested several dense neural network architectures to find the most effective model for the given task. Each experiment is organized into its own Jupyter Notebook for clarity. The following architectures have been explored:

1. **DNN Model 1: Basic Dense Layers**
    - Architecture: [describe the architecture]
    - Results: [include key metrics and insights]

2. **DNN Model 2: Adding Dropout for Regularization**
    - Architecture: [describe the architecture with dropout layers]
    - Results: [include key metrics and insights]

3. **DNN Model 3: Fine-tuning Hyperparameters**
    - Architecture: [describe the architecture with optimized hyperparameters]
    - Results: [include key metrics and insights]

## Submission

The best-performing model will be submitted to the Kaggle competition for evaluation. Results and leaderboard rankings will be updated accordingly.

## Getting Started

1. Clone this repository:

    ```bash
    git clone https://github.com/your-username/kaggle-neural-network-experiments.git
    ```

2. Navigate to the project directory:

    ```bash
    cd kaggle-neural-network-experiments
    ```

3. Install the required dependencies:

    ```bash
    pip install -r requirements.txt
    ```

4. Explore the Jupyter Notebooks in the `notebooks` directory to review the experiments.

## Acknowledgments

- This work is inspired by the Kaggle community and the valuable insights shared by fellow participants.
- Special thanks to Kaggle for hosting this playground competition and providing an opportunity for experimentation.

## License

This project is licensed under the [MIT License](LICENSE).
