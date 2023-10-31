# Bocah Mobile Legend Detection using TensorFlow and Keras

## Project Overview

This project aims to classify a mobile legend player based on their comments using deep learning natural language processing techniques implemented with TensorFlow Keras. The goal is to create a robust binary classification model that can accurately classify if the writer of the commment is a mobile legend player or not.

## Dataset

The dataset used for this project can be found [here](https://drive.google.com/file/d/1i69ONNTpJ8vadzH0phnoT--6cGsSmWr2/view?usp=drive_link). It consists of livestream and youtube comment chat from mobile legend or non-mobile legend(genshin impact, valorant, honkai star rail) livestream/video. The label of the dataset consist of '1' for mobile legend player and '0' for non-mobile legend player Ensure that you have downloaded and preprocessed the dataset as required before running the code or you can use the dataset that i provided on this repository.

Dataset contains :<br>
There are 463 sentences for training.<br>
There are 463 labels for training.<br>
There are 116 sentences for validation.<br>
There are 116 labels for validation.<br>


## Model Architecture

The deep learning model is built using the TensorFlow Keras libraries. The architecture typically involves:

- Preprocessing the datasets(drop duplicate, tokenizing, padding).
- Creating embedding layer with one layer of convulutional 1D layers then add GlobalAveragePooling, and add dense layers.
- Compiling the model with an appropriate loss function and optimizer.
- Training the model on the dataset.

You can find the detailed architecture and code in the Jupyter Notebook or Python script provided in this repository.

## Training Result
### training and validation acccuracy graph
![image](https://github.com/Benedixx/Bocah-Mobile-Legend-Detection/assets/97221880/3fce62d5-a77e-4177-9d97-6ed3b5333fb7)

### training and validation loss graph
![image](https://github.com/Benedixx/Bocah-Mobile-Legend-Detection/assets/97221880/d22701d5-9a24-404f-bcf1-c85cba7e21dd)


### training and validation acccuracy on last epoch
```bash
Epoch 50/50
15/15 [==============================] - 0s 10ms/step - loss: 0.2315 - accuracy: 0.8575 - val_loss: 0.2313 - val_accuracy: 0.9052
```
