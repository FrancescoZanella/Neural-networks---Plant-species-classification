# Plant Species Classification - README

## Problem Description
The task is to classify images of plants into eight different species categories. Each category corresponds to a specific plant species. The goal is to build a machine learning model that can predict the correct class label for a given image. 

## Dataset Details
You can download the dataset [here](https://drive.google.com/drive/u/0/folders/1JpHs0m-6IwI_cMUZ4cT5vlrBQyduwjFt)
- **Image Size**: 96x96 pixels
- **Color Space**: RGB
- **File Format**: JPG
- **Number of Classes**: 8
- **Classes**:
  
    0. Species1
    1. Species2
    2. Species3
    3. Species4
    4. Species5
    5. Species6
    6. Species7
    7. Species8

## Dataset Structure
The dataset is organized in a single folder named "training," which contains 3542 images. These images are already divided into sub-folders, each corresponding to a specific class. The distribution of training images per class is as follows:

- Species1: 186 images
- Species2: 532 images
- Species3: 515 images
- Species4: 511 images
- Species5: 531 images
- Species6: 222 images
- Species7: 537 images
- Species8: 508 images

## Code Overview
The provided Python code aims to address the plant species classification task. Here's a high-level overview of the code's structure and the approach used:

1. **Setup and Dependencies**
   - The code begins by importing necessary libraries and setting up the environment.
   - It installs the `keras_tuner` package and imports various TensorFlow and Keras components.

2. **Data Loading and Preprocessing**
   - The code loads and preprocesses the dataset using TensorFlow utilities.
   - It applies data augmentation techniques to the training dataset to improve model generalization.
   
3. **Model Building**
   - The code defines a neural network model for plant species classification.
   - It starts with a convolutional base followed by fully connected layers.
   - The model uses transfer learning with Xception and fine-tuning of layers.

4. **Training**
   - The code trains the model using the training dataset.
   - Training includes an early stopping callback to prevent overfitting.
   - Three phases of training are conducted: base model, fine-tuning all layers, and fine-tuning specific layers.

5. **Keras Tuner**
   - The code uses Keras Tuner to search for optimal hyperparameters for model training.
   - It defines a hyperparameter search space and performs a search to find the best hyperparameters.

## How to Use the Code
1. Ensure you have the required Python libraries installed, especially TensorFlow, Keras, and Keras Tuner.

2. Organize your dataset into the structure described in the "Dataset Structure" section.

3. Open the provided Python code in a compatible environment (e.g., Jupyter Notebook, Google Colab).

4. Run the code step by step, following the order described in the code.

5. After training, you can use the trained model for plant species classification on new images.

## Report
For more details about the model you can read the [report](https://github.com/FrancescoZanella/Neural_networks_Plant_species_classification/blob/main/REPORT_HOMEWORK1.docx), where everyting is explained in detail.


## Conclusion
This code is designed to address the plant species classification task with the provided dataset for ANNDL course challenge [here](https://codalab.lisn.upsaclay.fr/competitions/8522) at polimi.
My team have received 5.5 out of 5.5 points doing this challenge.

