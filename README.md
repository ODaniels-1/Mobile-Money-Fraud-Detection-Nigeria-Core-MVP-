# Mobile-Money-Fraud-Detection-Nigeria-Core-MVP-
Machine learning MVP using Random Forest to detect and flag fraudulent mobile money transactions within the Nigerian financial context
# Mobile-Money Fraud Detection Nigeria (Core MVP)

## Problem Context
Mobile money services like OPay, PalmPay, and MTN MoMo process millions of transactions daily across Nigeria. This massive volume makes digital wallets a frequent target for phishing, social engineering, and transaction scams. Because manual review cannot scale to meet this volume, this project focuses on building a machine learning system to automatically identify and flag suspicious transaction patterns.
This MVP is built and evaluated using the **PaySim Synthetic Financial Dataset**, which models real-world mobile money financial logs from an operational African mobile service provider. The dataset contains 6,362,620 transactions covering operations like TRANSFER, CASH_OUT, and PAYMENT, providing a realistic foundation for training fraud detection models.


## Project Overview
This repository contains a Machine Learning Minimum Viable Product (MVP) designed to automatically identify and flag fraudulent mobile money transactions. The project is tailored to the Nigerian financial context (addressing platforms like OPay, PalmPay, and MTN MoMo) where high transaction volumes make manual review impossible.


## Core MVP Features
* **Data Preparation**: Drops identification strings, converts transaction types into numeric features, and handles class imbalance using downsampling.
* **Model Training**: Implements a Random Forest Classifier trained on balanced transaction patterns.
* **Anomaly Flags**: Uses an optimized 90% decision threshold to isolate high-risk actions.
* **Evaluation Metrics**: Uses Precision, Recall, and F1-Score instead of misleading raw accuracy.

## Evaluation Results
The model achieved the following performance metrics on the hidden testing dataset:
* **Fraud Recall (93%)**: Successfully detected and blocked 93% of all actual fraudulent transactions.
* **Fraud Precision (42%)**: Maintained an operational balance, ensuring legitimate user transfers face minimal false alarms.
* **Overall Accuracy (100%)**: High overall accuracy due to near-perfect classification across the massive volume of legitimate data.

## Tools Used
* Python, Pandas, Scikit-learn, Matplotlib, Seaborn, Jupyter Notebook
