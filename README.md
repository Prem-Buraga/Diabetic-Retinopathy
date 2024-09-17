# Diabetic Retinopathy Detection Using Deep Learning

## Overview

This project focuses on detecting diabetic retinopathy in retinal images. It includes data preprocessing, exploratory data analysis (EDA), deep learning model training (including custom Deep Convolutional Neural Network (DCNN) and AlexNet), and performance evaluation. The project also features a frontend application (`app.py`) where users can upload retinal images and view detection results.

## Table of Contents
- [Dataset](#dataset)
- [Frontend Application](#frontend-application)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Data Preprocessing](#data-preprocessing)
- [Modeling](#modeling)
- [Deep Convolutional Neural Network (DCNN)](#deep-convolutional-neural-network-dcnn)
- [AlexNet](#alexnet)
- [Training](#training)
- [Evaluation](#evaluation)
- [Results](#results)
- [Contributing](#contributing)
- [License](#license)

## Dataset

The dataset for diabetic retinopathy detection can be downloaded from the [Kaggle APTOS 2019 Blindness Detection competition page](https://www.kaggle.com/c/aptos2019-blindness-detection/data). Extract the dataset and place it in the `Dataset` directory of the project.

## Frontend Application

The project includes a frontend implemented using Flask, which allows users to upload retinal images for diabetic retinopathy detection. To successfully run the project:

1. Create a folder named `templates` in the project directory.
2. Place the `index.html` and `result.html` files inside the `templates` folder.
3. Run the `app.py` file to launch the Flask web application.

The application will display both the uploaded image and the detected result.

## Exploratory Data Analysis

Exploratory Data Analysis (EDA) includes:

- Loading and inspecting the data.
- Checking for class imbalances.
- Visualizing the distribution of the target variable (different stages of diabetic retinopathy).

## Data Preprocessing

The preprocessing stage includes:

- **Augmenting** the minority classes to balance the dataset.
- **Resizing** and **normalizing** the retinal images to prepare them for model input.

## Modeling

Two models are implemented for comparison:

### Deep Convolutional Neural Network (DCNN)
A custom DCNN is built for classifying retinal images. The model consists of several convolutional and max-pooling layers, followed by fully connected dense layers.

### AlexNet
The AlexNet architecture is also implemented for comparison, with a series of convolutional layers followed by fully connected layers.

## Training

The models are trained using the preprocessed dataset. The dataset is split into training and validation sets. The training process is conducted over multiple epochs, with real-time evaluation using the validation data.

## Evaluation

Performance is evaluated using accuracy, loss metrics, and confusion matrices. These metrics help assess the model's classification performance across different severity levels of diabetic retinopathy.

## Results

The final performance results of the models are visualized through accuracy and loss plots. The classification report provides a detailed evaluation.
![image](https://github.com/user-attachments/assets/d20c40cb-dd63-4ee5-8515-fd2563fd44aa)

![image](https://github.com/user-attachments/assets/a7b2408b-1c1d-488a-a0ae-a6338d7c544a)



- **Final Accuracy after 6 epochs**: 97.43%

## Contributing

Contributions to the project are welcome! To contribute:

1. Fork the repository.
2. Create a new branch for your changes.
3. Commit and push your changes.
4. Submit a pull request.

For feature requests or issues, please open an issue on GitHub.


---

Feel free to customize this documentation to suit your specific needs.
