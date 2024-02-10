Potato Disease Classification using TensorFlow
This repository contains code for a potato disease classification model using TensorFlow. The model is designed to classify potato plant images into three categories: 'Potato___Early_blight', 'Potato___Late_blight', and 'Potato___healthy'.

Dataset
The dataset used for training the model is sourced from the PlantVillage dataset and consists of 2152 images belonging to the three mentioned classes.

Getting Started
Ensure you have TensorFlow installed:

bash
Copy code
pip install tensorflow
Download the dataset from PlantVillage and extract it to the specified directory

Run the provided code in a Python environment with the required dependencies installed.

Model Architecture
The model architecture consists of several convolutional and pooling layers, followed by fully connected layers. The model is compiled using the Adam optimizer and Sparse Categorical Crossentropy loss function.

Training
The dataset is split into training, validation, and test sets. The model is trained for 10 epochs, and training progress is visualized with training and validation accuracy/loss plots.

Quantization
Quantization is applied to the trained model using TensorFlow Model Optimization library. The quantized model is then converted to a TensorFlow Lite model for deployment on resource-constrained devices.

Evaluation
The model and quantized model are evaluated on the test set, and accuracy scores are displayed. The quantized TensorFlow Lite model is saved for deployment.

Inference
Inference is demonstrated on a sample of images from the test set. Predictions are made, and the actual and predicted classes, along with confidence percentages, are visualized.

Files and Directories
potato_disease_classification.ipynb: Jupyter Notebook containing the complete code.
models/: Directory to save the quantized TensorFlow Lite model.
PlantVillage/: Directory containing the PlantVillage dataset.
Feel free to explore, modify, and use this code for your own projects related to image classification tasks. If you encounter any issues or have suggestions for improvement, please feel free to open an issue or submit a pull request. Happy coding!
