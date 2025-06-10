# Fraud Detection Using Reinforcement Learning

This repository contains a reinforcement learning model designed to detect fraudulent transactions in credit card data. The project explores the application of RL techniques to identify anomalies and improve the accuracy of fraud detection systems.

## Team Members:

* Abdenour Bouziane
* Abderrahim Rezki
* Mohcen Tahar Chouireb
* Mohammed Chaker Baaziz
* Marouane Abdeldjalil Ouled Ali

## Project Overview

Traditional fraud detection methods often rely on supervised learning, which can be limited by imbalanced datasets and the evolving nature of fraudulent activities. This project investigates the use of Reinforcement Learning (RL) as a dynamic and adaptive approach to fraud detection. The core idea is to train an agent to learn optimal strategies for identifying fraudulent transactions by interacting with an environment representing transaction data.

## Dataset

The dataset used in this project is the [Credit Card Fraud Detection](https://www.kaggle.com/datasets/dalpozz/creditcardfraud) dataset available on Kaggle. This dataset contains transactions made by European cardholders in September 2013. It presents transactions that occurred in two days, where we have 492 frauds out of 284,807 transactions. The dataset is highly unbalanced, with the positive class (frauds) accounting for 0.172% of all transactions.

## Methodology

The project implements a reinforcement learning framework, likely involving:

* **Environment Definition:** Creating a simulation environment that mimics credit card transactions, where the agent receives states (transaction features) and takes actions (classifying as fraudulent or legitimate).
* **Agent Design:** Developing an RL agent (e.g., using Q-learning, SARSA, or Deep Q-Networks) capable of learning from rewards and penalties associated with correct and incorrect classifications.
* **Reward Structure:** Defining a reward system that encourages the agent to correctly identify fraudulent transactions while minimizing false positives.
* **Exploration Strategies:** Implementing techniques to balance exploration (discovering new strategies) and exploitation (using learned strategies) during training.
* **Model Training and Evaluation:** Training the RL model on the provided dataset and evaluating its performance using appropriate metrics for imbalanced datasets (e.g., precision, recall, F1-score, ROC-AUC).

## Key Findings and Future Work

The notebook likely details the experimental setup, results, and analysis of the RL model's performance in fraud detection. Key findings may include insights into the effectiveness of RL in handling imbalanced data and adapting to new fraud patterns.

Future work could explore:

* More advanced RL techniques, such as hierarchical reinforcement learning or multi-agent systems.
* Integration with real-time transaction streams for continuous learning.
* Investigation of different feature engineering strategies to enhance the agent's perception of fraudulent activities.
* Robustness analysis against adversarial attacks.

## Getting Started

To run the notebook and reproduce the results, you will need:

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/your-username/your-repo-name.git](https://github.com/your-username/your-repo-name.git)
    cd your-repo-name
    ```
2.  **Download the dataset:**
    The dataset can be downloaded directly from Kaggle: [Credit Card Fraud Detection](https://www.kaggle.com/datasets/dalpozz/creditcardfraud). Place the `creditcard.csv` file in the appropriate directory (as expected by the notebook).
3.  **Install dependencies:**
    It is recommended to use a virtual environment.
    ```bash
    pip install -r requirements.txt # (Assuming a requirements.txt file will be created)
    ```
    *If no `requirements.txt` is provided, commonly used libraries for this type of project include:*
    ```bash
    pip install numpy pandas scikit-learn tensorflow # or pytorch if deep learning is used
    ```
4.  **Open and run the Jupyter Notebook:**
    ```bash
    jupyter notebook "Credit Card Fraud Detection.ipynb"
    ```
