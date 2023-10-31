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
- Creating embedding layer with one layer of convulutional 1D layers then add GlobalAveragePooling, and add another dense layers.
- Compiling the model with an appropriate loss function and optimizer.
- Training the model on the dataset.

You can find the detailed architecture and code in the Jupyter Notebook or Python script provided in this repository.

## Training Result
### training and validation acccuracy graph
![image](https://github.com/Benedixx/Brain-Tumor-Classification/assets/97221880/e4b658b1-8bcb-481e-ab62-e1189638554d)


### training and validation acccuracy on last epoch
```bash
Epoch 21/25
20/20 [==============================] - 2s 101ms/step - loss: 0.5212 - accuracy: 0.7688 - val_loss: 0.5506 - val_accuracy: 0.7917 - lr: 1.2500e-04
```
## Improvement

### Add predict input data

The model can be used but there is no input predict after the model training, you can contribute to add the input predict.

### Need to improve the accuracy
The model accuracy can be improved, but since i have another deadline :3 and it takes a long time i have to temporarily stop. UwU
