# Hand-Gesture-Recognition-using-Convolutional-Neural-Network-CNN-

# Hand Gesture Recognition using Convolutional Neural Network (CNN)

This project implements a Convolutional Neural Network (CNN) to classify hand gestures from images. The model is trained on the Leap Gesture Dataset, which contains 10 different hand gesture categories, enabling intuitive human-computer interaction for gesture-based control systems.

## Dataset
The dataset used is the [Leap Gesture Dataset](https://www.kaggle.com/datasets/gti-upm/leapgestrecog) from Kaggle. The dataset includes 10 categories:
- 01_palm
- 02_l
- 03_fist
- 04_fist_moved
- 05_thumb
- 06_index
- 07_ok
- 08_palm_moved
- 09_c
- 10_down

### Directory Structure
project_folder/ ├── leapGestRecog/ # Dataset │ ├── 01_palm/ │ ├── 02_l/ │ ├── 03_fist/ │ └── ... ├── src/ │ ├── train_model.py # Code for training and evaluating the model │ ├── visualize.py # Visualization of results and confusion matrix ├── README.md └── requirements.txt


### Model Architecture
The model is a CNN implemented using Keras, consisting of the following layers:
- **Convolutional Layers**: Three Conv2D layers with ReLU activation and MaxPooling.
- **Dropout Layers**: To prevent overfitting.
- **Fully Connected Layer**: Dense layer with ReLU activation.
- **Output Layer**: Softmax layer with 10 classes (one for each gesture).

### Requirements
Install dependencies by running:

pip install -r requirements.txt
Training and Evaluation
Run train_model.py to load, preprocess, train, and evaluate the CNN model:

python src/train_model.py
Results
The model achieved an accuracy of approximately 85% on the test set. Below are some evaluation metrics:

Confusion Matrix

Training and Validation Loss

Training and Validation Accuracy

Sample Predictions
Here are a few predictions made by the model:


License
This project is licensed under the MIT License. See LICENSE for details.


# Acknowledgments
Thanks to Kaggle and GTI-UPM for providing the dataset used in this project.



