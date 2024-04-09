# Melanoma Cancer Detection Project
> The aim of this project is to build a CNN based model which can accurately detect melanoma. Melanoma is a type of cancer that can be deadly if not detected early. It accounts for 75% of skin cancer deaths. A solution that can evaluate images and alert dermatologists about the presence of melanoma has the potential to reduce a lot of manual effort needed in diagnosis.


## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)


## General Information
- In this project we intend to use a set of 2357 images of malignant and benign oncological diseases, and create a model which can identify melanoma which is a type of cancer.
- Data Preprocessing:
   - Resized images to 180x180 pixels.
   - Created train and test datasets using TensorFlow's `image_dataset_from_directory` function.


## Conclusions
- Model Building:
   - Built a CNN model with 3 convolutional layers, 3 max pooling layers, and 1 dense layer.
   - Trained the model for 20 epochs and observed overfitting.

- Addressing Overfitting:
   - Added dropout and batch normalization layers to the model.
   - Trained the model again for 20 epochs, but overfitting persisted.

- Data Augmentation and Class Rebalance:
   - Used Augmentor library to generate additional images for each class to address class imbalance.
   - Created a new train dataset with augmented images.

- Model Building with Augmented Data:
   - Built a new CNN model with 4 convolutional layers, 4 max pooling layers, 4 normalization layers, and 1 dropout layer.
   - Trained the model for 30 epochs and achieved a validation accuracy of ~74%.

- Further Model Refinement:
   - Built another CNN model with 4 convolutional layers, 4 max pooling layers, and 2 dropout layers.
   - Trained the model for 30 epochs and achieved a validation accuracy of ~80%, which was the best result obtained.



## Technologies Used
* **Python:** The main programming language used for the project.
* **TensorFlow:** A popular deep learning library used for building and training the CNN model.
* **Keras:** A high-level API for building and training deep learning models with TensorFlow.
* **Augmentor:** A library used for image augmentation, which helped to address class imbalance and improve the model's performance.
* **NumPy:** A library used for numerical computations and array manipulations.
* **Pandas:** A library used for data analysis and manipulation.
* **Matplotlib:** A library used for creating visualizations.
* **Seaborn:** A library used for creating statistically-informed visualizations.
* **PIL:** A library used for image processing.

## Acknowledgements
- This project was inspired by UpGrad


## Contact
Created by [@AkashMSrivastava] - feel free to contact me!
