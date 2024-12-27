# MLOps New York Taxi Trip Duration Prediction

This project builds an end-to-end machine learning pipeline for predicting New York City taxi trip durations based on features such as pick-up/drop-off locations, time, distance, and more. It covers the entire machine learning lifecycle, from data ingestion and preprocessing to model training, hyperparameter tuning, and cloud deployment. The project follows MLOps best practices, including version control, CI/CD, model tracking, and containerization.

The pipeline uses technologies like AWS, Docker, DVC and GitHub Actions for scalability, reproducibility, and automation

## Table of Contents

- [Project Overview](#project-overview)
- [Technologies Used](#technologies-used)
- [Setup and Installation](#setup-and-installation)
- [Data Ingestion](#data-ingestion)
- [Data Preprocessing and Feature Engineering](#data-preprocessing-and-feature-engineering)
- [Model Training and Hyperparameter Tuning](#model-training-and-hyperparameter-tuning)
- [Model Evaluation](#model-evaluation)
- [Deployment with Fast API and Docker](#deployment-with-Fast-Api-and-docker)
- [CI/CD with GitHub Actions](#cicd-with-github-actions)
- [Cloud Deployment on AWS](#cloud-deployment-on-aws)
- [How to Run the Project](#how-to-run-the-project)
- [Licenses](#licenses)

---

## Project Overview

This project provides a solution for predicting the trip duration of New York taxis based on various features like pick-up and drop-off locations, time of day, distance, and more. The solution is implemented as a fully automated pipeline that includes:

- **Notebook Experiments**: I started by fetching the dataset and performing data cleaning, exploratory data analysis (EDA), and multicollinearity checks using hypothesis testing. I applied feature engineering, selection, and column transformers for categorical and numerical encoding, Min-Max scaling, Standard scaling, and other transformations. I also handled outliers and class imbalance. For better insights, I used various visualizations, including bar plots, heatmaps, scatter plots, and pair plots etc.
- **Data Ingestion**: Download and unzip data from the Kaggle competition dataset.
- **Data Preprocessing**: Correct data types, handle missing values, and perform categorical encoding.
- **Feature Engineering**: Transform features to improve model performance.
- **Model Training**: Train a machine learning model (RandomForest, DessionTrees, XGBoost etc) with hyperparameter tuning but XGBoost give me Best accuracy that's why final model i am using XGBoost model for deployment.
- **Model Evaluation**: Evaluate model performance using appropriate metrics.
- **Deployment**: Deploy the model using Fast Api for real-time predictions and Docker for containerization.
- **CI/CD**: Automate testing, deployment, and version control with GitHub Actions.
- **Cloud Deployment**: Deploy the solution on AWS using EC2 and ECR.

---

## Technologies Used

- **Data Processing**: Pandas, NumPy, Scikit-learn
- **Data Versioning**: DVC (Data Version Control)
- **Modeling**: XGBoost, and also training another model.But best accuracy i got XGBoost model.
- **Web App**: Fast API
- **Containerization**: Docker
- **CI/CD**: GitHub Actions
- **Cloud**: AWS (EC2, ECR, S3)
- **Other Tools**: Git, pytest

---

## Setup and Installation

1. **Clone the repository**:
   ```bash
   git clone https://github.com/JahidHasan010/MLOps-NEW-YORK-TAXI-TRIP-DURATION.git
   cd MLOps-NEW-YORK-TAXI-TRIP-DURATION
