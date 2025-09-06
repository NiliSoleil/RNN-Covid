# RNN-Covid
RNN-Covid

COVID-19 Prediction with Recurrent Neural Networks

This repository contains a deep learning project focused on time series prediction using various Recurrent Neural Network (RNN) architectures. The project uses a dataset of confirmed COVID-19 cases to predict future trends.

Project Objectives

The main goals of this project were to:

  Data Preparation: 📊 To prepare time series data for an RNN model, including normalization and creating sequential samples.
  Model Implementation: 🧠 To implement and compare the performance of different RNN models, including custom and built-in PyTorch versions.
  Model Evaluation: 📉 To evaluate the models' performance using the MAE metric and visualize their predictions against the actual data.
  
Key Project Steps

The project was completed in the following stages:

**1. Dataset Preparation**
  
  📚 The dataset was loaded from the data folder, which contains 327 samples, each with a sequence length of 5. This means that 5 consecutive days of data are used to predict the value on the 6th day.
  
  🔪 The dataset was split into three sections: Training (80%), Evaluation (10%), and Testing (10%).
  
  ✨ The data was normalized using a standard normalization method to improve model performance.
  
**2. Neural Network Model Definition**
  
  Custom Models: 🧠 A custom model was created that takes the type of RNN as an input. This was used to evaluate and compare the performance of pre-built RNN, LSTM, and GRU models from PyTorch.
 
  A separate CNNLSTM custom model was built, which includes a 1D convolutional layer followed by an LSTM layer with a hidden state of 4.
  
  Custom GRU Implementation: 🛠️ A GRU network was implemented from scratch to demonstrate an understanding of its internal mechanics. The output of this model was checked with random data.
  
**3. Device Selection**
  
  🚀 The models were moved to a GPU for accelerated training.
  
**4. Loss Function and Optimizer**
  
  📉 The L1 Loss function and the Adam optimizer were defined.
  
**5. Model Training and Evaluation**
  
  🏋️ Each of the defined models (RNN, LSTM, GRU, and CNNLSTM) was trained using the best practices for hyperparameter selection.
  
  📊 The learning curve (loss vs. epochs) was plotted for each model to visualize training progress.
  
  📈 The MAE (Mean Absolute Error) metric was calculated for each model on the entire test dataset, and the results were recorded in a table for comparison.
  
**6. Model Testing and Visualization**
  
  🖼️ A graph was plotted to compare the predicted output of the models against the actual values from the test dataset.
  
**7. Optional Task: Time Series Data Formatting**
  
  💡 For additional practice, the raw cases_daily dataset (a 332x1 vector) could be used to create sequential data with a window length of 5, which would then be used for training a new model.

**How to Run the Code**

  **Prerequisites:** 🛠️ Make sure you have the necessary libraries, such as PyTorch, installed.
  **Run the Notebook:** 🖥️ The code is available here: https://github.com/NiliSoleil/RNN-Covid/blob/main/RNN_LSTM_GRU.ipynb

You can run it in Google Colab or any Jupyter environment.

Niloufar Soleil


