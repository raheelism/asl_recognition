# American Sign Language (ASL) Prediction Using CNN

## Overview

This project aims to classify images of American Sign Language (ASL) letters using a Convolutional Neural Network (CNN). ASL is a rich language used primarily by deaf individuals in North America and involves hand signs, facial gestures, and bodily postures. The project focuses on classifying individual letters rather than sentences, serving as a foundational step towards more complex translation systems.

## Dataset

The dataset consists of images of ASL letters 'A', 'B', and 'C'. The data is split into training and test sets:
- `x_train` and `x_test`: Arrays of image data with shape `(num_samples, 3, 50, 50)`.
- `y_train` and `y_test`: Arrays of category labels with shape `(num_samples,)`.

## Project Steps

1. **Data Loading and Visualization**:
   - The training and test datasets are loaded.
   - The first several images along with their labels are visualized.

2. **Dataset Examination**:
   - The number of images for each letter in the training and test datasets is examined to ensure balanced classes.

3. **One-hot Encoding**:
   - The labels are one-hot encoded to prepare them for input into a Keras model.

4. **Model Definition**:
   - A CNN model is defined with convolutional layers, max pooling layers, and a dense output layer.

5. **Model Compilation**:
   - The model is compiled using the RMSprop optimizer and categorical cross-entropy loss function.

6. **Model Training**:
   - The model is trained on the training data with a validation split of 20% and for 2 epochs.

7. **Model Testing**:
   - The model's performance is evaluated on the test dataset to measure its accuracy.

8. **Visualization of Mistakes**:
   - Misclassified images are visualized to understand potential challenges in classification.

## Requirements

- Python 3.x
- TensorFlow
- Keras
- NumPy
- Matplotlib

## Usage

1. Clone the repository.
2. Install the required packages.
3. Run the Jupyter notebook to train and evaluate the model.

## Results

The model achieves high accuracy on the test dataset, indicating effective learning and generalization. Misclassified images are analyzed to identify potential areas for model improvement.

## Future Work

- Expand the dataset to include more ASL letters.
- Experiment with different network architectures and hyperparameters.
- Develop a system for real-time ASL translation using video input.

## License

This project is licensed under the MIT License.
