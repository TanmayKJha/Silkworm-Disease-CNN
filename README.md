# Disease Detection in Bombyx Mori Using Convolutional Neural Networks (CNN)

**Overview**
This project implements a deep learning-based approach to classify images of Bombyx Mori silkworms into Diseased and Undiseased categories. By leveraging Convolutional Neural Networks (CNNs), the model achieves high accuracy, making it a reliable solution for early disease detection in sericulture.

**Dataset**
Source: Dataset of 492 images belonging to two classes: Diseased and Undiseased.

**Preprocessing:**
-Images resized to 250x250 pixels.
-Normalized pixel values (scaled between 0 and 1).
-Augmented with random flips and rotations for better generalization.

**Model Architecture**
The CNN architecture includes:

-Resizing and Rescaling Layers: Normalize images for consistent input.
-Data Augmentation Layers: Add variability to the training data.
-Convolutional Layers: Extract spatial features using filters.
-Pooling Layers: Reduce dimensionality and computational load.
-Fully Connected Layers: Perform final classification using dense layers with ReLU and Softmax activation.

**Model Summary:**

-Input Shape: (8, 250, 250, 3)
-Output Classes: 2 (Diseased, Undiseased)
-Total Parameters: 168,195

**Training and Results**

-Optimizer: Adam
-Loss Function: Sparse Categorical Crossentropy
-Metrics: Accuracy

**Performance:**
-Training Accuracy: 99.74%
-Validation Accuracy: 100%
-Test Accuracy: 95.83%

**Key Features**
-Automated disease classification with high accuracy.
-Lightweight model architecture, suitable for deployment.
-Training and validation accuracy plots to visualize performance.

**How to Use**

Clone the Repository:
->git clone https://github.com/TanmayKJha/BombyxMori-DiseaseDetection.git  
cd BombyxMori-DiseaseDetection  

Install Dependencies:
->pip install -r requirements.txt  

Run Training Script:
->python train.py  

Evaluate Model:
->python evaluate.py  
