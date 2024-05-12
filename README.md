# Real-Time-Sign-Language-Detection

Welcome to the GitHub repository for our ASL Detection System, developed as part of the "Introduction to Machine Learning (IML)" course. This project utilizes a convolutional neural network (CNN) to recognize American Sign Language (ASL) gestures in real-time, enhancing communication for the deaf and hard-of-hearing community.

## Project Team
- Adoksh M Bhardwaj
- Ajay S Prakash
- K Jaidev Shankar Reddy
- Manvitha R Kabbathi

## Project Structure

This repository is organized into several sections:
1. **Data Collection**
2. **Data Preparation**
3. **Model Training**
4. **Real-Time Detection**
5. **Dataset**

## Step-by-Step Guide

### 1. Data Collection
To collect the ASL gesture images, use the `collectdata.py` script. This script utilizes a webcam to capture images of ASL gestures when a specific key corresponding to each letter is pressed. Ensure you have a webcam connected and operational before starting this step.

**Usage:**
```bash
python collectdata.py
```

### 2. Data Preparation
Once data collection is complete, organize the data into training and validation sets using the `split.py` script. The data is split in the ratio of 0.8 for training and 0.2 for validation. This will help in training the model effectively by providing a set of unseen images for validating the model's performance.

**Usage:**
```bash
python split.py
```
Make sure to paste the training and validation paths in the `trainmodel-2.ipynb` for proper model training.

### 3. Model Training
Train the CNN using the `trainmodel-2.ipynb` Jupyter notebook. This notebook outlines the structure of the CNN and contains code for training the model on the collected data. After training, the model architecture is saved as a JSON file and the model weights as an H5 file. Ensure you have Jupyter Notebook installed to open and run this file.

**Usage:**
Open and run the notebook in Jupyter:
```bash
jupyter notebook trainmodel-2.ipynb
```

### 4. Real-Time Detection
After training the model, use the `realtimedetection.py` script to start the real-time detection of ASL gestures. This script loads the trained model using the JSON file and H5 file paths provided. It uses the webcam to detect and classify ASL gestures live.

**Usage:**
```bash
python realtimedetection.py
```

### 5. Dataset
The dataset used for training and validation, consisting of 4,466 ASL gesture images, is included in this repository. It is divided into training and validation sets, with detailed organization in the dataset directory.

## Requirements
- Python 3.8+
- Libraries: OpenCV, TensorFlow, Keras, NumPy
- Jupyter Notebook or Google Colab for running `.ipynb` files

## Installation
Clone this repository to your local machine:
```bash
git clone Repository Link 
```
Install the required libraries:
```bash
pip install -r requirements.txt
```

## Thank You
