image-classification-orange-Image Classification with Orange
Overview This project demonstrates how to classify images into two categories: is_building and is_not_building. The analysis uses the Orange Data Mining Tool and a dataset from Kaggle. The process involves data preprocessing, embedding generation, unsupervised clustering, and supervised classification with multiple models.

Table of Contents Goal Dataset Data Preparation Methods Results Conclusion Goal The primary objective of this analysis is to identify whether a given image contains a building or not.

Dataset The dataset used for this project is from Kaggle: Intel Image Classification Dataset. It consists of images categorized into six groups:

Buildings Forest Glacier Mountain Sea Street Key Information Total Images: ~25,000 Image Dimensions: 150x150 pixels Categories: 6 rust Copy Edit {'buildings' -> 0, 'forest' -> 1, 'glacier' -> 2, 'mountain' -> 3, 'sea' -> 4, 'street' -> 5} Data Preparation To prepare the dataset for analysis:

Split Data: The images were divided into: Training Set: 204 images Test Set: 50 images Orange Workflow: Orange recognized two categories for the analysis: is_building and is_not_building. An Image Embedding was created using the VGG-16 model, pre-trained on ImageNet, to make the data suitable for machine learning models. Methods Clustering Unsupervised Learning: The Distances and Hierarchical Clustering widgets were used to visualize clusters in the data. Classification Supervised Learning Models:

Test and Score Widget evaluated the following models: Logistic Regression Naïve Bayes Neural Network Workflow Configuration:

Training data was connected to the Image Embedding. Test data predictions were visualized using the Predictions Widget. Results The evaluation of the three models yielded the following results:

Logistic Regression achieved the highest accuracy. A Confusion Matrix confirmed the advantage of Logistic Regression over the other models. Workflow Screenshots Training Data Clustering

Model Evaluation

Logistic Regression Predictions

Conclusion Logistic Regression outperformed other models in identifying buildings. Orange's tools for embedding and clustering enabled efficient preprocessing and analysis. The project showcases the utility of Orange in image classification tasks. How to Use This Repository Install Orange: Orange Installation Guide

Download Dataset: Intel Image Classification on Kaggle

Replicate Workflow:

Open Orange. Load the dataset and replicate the steps described in the Methods section. References Orange Data Mining Documentation Intel Image Classification Dataset on Kaggle Notes Replace the path/to/cluster-analysis.png and similar placeholders with the actual image paths or upload them to your repository and link accordingly.
