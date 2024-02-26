# Parkinson-Disease-Detection
The Parkinson's Disease Detection project utilizes the Oxford Parkinson's Disease dataset with 197 instances and 23 real-valued attributes. Conducting classification tasks, the project employs machine learning models to discriminate between healthy individuals and those with Parkinson's disease based on biomedical voice measurements, contributing to the diagnosis and understanding of the disease.

## Dataset Overview
The Parkinson's Disease dataset consists of biomedical voice measurements from 31 individuals, 23 with Parkinson's disease (PD). There are 197 instances, with each row corresponding to a voice recording. The dataset includes 23 real-valued attributes, such as vocal fundamental frequency measures, variation in frequency and amplitude, noise-to-tonal component ratios, and nonlinear complexity measures. The goal is to discriminate between healthy subjects (status=0) and those with PD (status=1). Recorded by Max Little in collaboration with the National Centre for Voice and Speech, the dataset is valuable for classification tasks. It is in ASCII CSV format and has been utilized in a study focusing on telemonitoring PD. 

![image](https://github.com/amiruzzaman1/Parkinson-Disease-Detection/assets/68743925/c6c2f74d-0a8a-448f-91f3-673a8c593d8d)
![image](https://github.com/amiruzzaman1/Parkinson-Disease-Detection/assets/68743925/cae9ae8b-e0e4-48b5-aacb-2d88bf68b749)
![image](https://github.com/amiruzzaman1/Parkinson-Disease-Detection/assets/68743925/5f2abb72-7fe4-4b43-bf86-826e9bb3a8b1)
![image](https://github.com/amiruzzaman1/Parkinson-Disease-Detection/assets/68743925/c9deaefb-b1ee-452b-ab26-1d5d7d8023b9)
![image](https://github.com/amiruzzaman1/Parkinson-Disease-Detection/assets/68743925/eb1c9b3d-fa7e-4a15-8de3-0b4711d9b285)

**Dataset Link:** [Parkinson's Disease Dataset](https://www.kaggle.com/datasets/thecansin/parkinsons-data-set)

## Colab Notebook

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1pN57nSx-5-xTLIvJ3kX61lqD03M2pOGU?usp=sharing)

## Models and Results

| Model                         | Accuracy   | Precision (Class 0) | Recall (Class 0) | F1-Score (Class 0) | Precision (Class 1) | Recall (Class 1) | F1-Score (Class 1) |
|-------------------------------|------------|----------------------|------------------|--------------------|----------------------|------------------|--------------------|
| **SVM**                       | 0.87       | 0.67                 | 0.57             | 0.62               | 0.91                 | 0.94             | 0.92               |
| **Random Forest**             | 0.95       | 1.00                 | 0.71             | 0.83               | 0.94                 | 1.00             | 0.97               |
| **K-Nearest Neighbors**       | 0.95       | 1.00                 | 0.71             | 0.83               | 0.94                 | 1.00             | 0.97               |
| **Logistic Regression**       | 0.90       | 1.00                 | 0.43             | 0.60               | 0.89                 | 1.00             | 0.94               |
| **Decision Tree**             | 0.92       | 0.83                 | 0.71             | 0.77               | 0.94                 | 0.97             | 0.95               |
| **Gradient Boosting**         | 0.92       | 0.83                 | 0.71             | 0.77               | 0.94                 | 0.97             | 0.95               |
| **LSTM**                       | 0.95       | 1.00                 | 0.71             | 0.83               | 0.94                 | 1.00             | 0.97               |
| **BiLSTM**                     | 0.95       | 1.00                 | 0.71             | 0.83               | 0.94                 | 1.00             | 0.97               |
| **CNN**                        | 0.87       | 0.75                 | 0.43             | 0.55               | 0.89                 | 0.97             | 0.93               |
| **Naive Bayes**                | 0.72       | 0.33                 | 0.57             | 0.42               | 0.89                 | 0.75             | 0.81               |
| **CNN + GRU**                  | 0.85       | 0.57                 | 0.57             | 0.57               | 0.91                 | 0.91             | 0.91               |
| **CNN + LSTM**                 | 0.87       | 0.62                 | 0.71             | 0.67               | 0.94                 | 0.91             | 0.92               |
| **LSTM + GRU**                 | 0.95       | 1.00                 | 0.71             | 0.83               | 0.94                 | 1.00             | 0.97               |
| **LSTM + GRU (ROS)**           | 1.00       | 1.00                 | 1.00             | 1.00               | 1.00                 | 1.00             | 1.00               |
| **CNN + LSTM (ROS)**           | 1.00       | 1.00                 | 1.00             | 1.00               | 1.00                 | 1.00             | 1.00               |
| **XGB-NN Hybrid (ROS)**        | 1.00       | 1.00                 | 1.00             | 1.00               | 1.00                 | 1.00             | 1.00               |
| **XGB-NN Hybrid (Undersample)**| 1.00       | 1.00                 | 1.00             | 1.00               | 1.00                 | 1.00             | 1.00               |
| **CNN + LSTM (Undersample)**   | 0.85       | 0.79                 | 1.00             | 0.88               | 1.00                 | 0.67             | 0.80               |
| **LSTM + GRU (Undersample)**   | 0.70       | 0.73                 | 0.73             | 0.73               | 0.67                 | 0.67             | 0.67               |

Note: ROS stands for Random Oversampling, and the same applies for Undersample.


