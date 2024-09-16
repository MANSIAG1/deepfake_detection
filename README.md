•This project is a deepfake detection system built using deep learning techniques. The system uses MobileNetV2 as a feature extractor and a custom neural network for classification.
The application includes a training script and a Streamlit-based web application for inference

Project Structure

Deepfake-Detection-Project/
├── app.py                      # Streamlit web app for deepfake detection
├── predict.py                  # Standalone script for image prediction
├── train.py                    # Script for training the deepfake detection model
├── test_imports.py             # Script to verify imports
├── deepfake_detection_model.h5 # Pre-trained model
├── requirements.txt            # Python dependencies
├── README.md                   # Documentation

Installation
Clone the repository:

git clone [https://github.com/yourusername/Deepfake-Detection-Project.git](https://github.com/MANSIAG1/deepfake_detection)
cd Deepfake-Detection-Project
Install dependencies: Make sure you have Python 3.6+ installed. Then, install the required libraries:

pip install -r requirements.txt

Scripts
train.py
This script trains the deepfake detection model using MobileNetV2. It performs the following tasks:
Loads and preprocesses images from the specified directories.
Applies data augmentation.
Builds and trains a MobileNetV2-based model.
Saves the trained model to deepfake_detection_model.h5.
Visualizes training and validation accuracy and loss.


predict.py
This script is used for making predictions on images. It loads the trained model and predicts whether the given image is real or fake.


app.py
This is a Streamlit-based web application for interactive deepfake detection. It allows users to upload an image and get real-time predictions on whether the image is fake or real.


test_imports.py
This script verifies that the essential libraries are installed correctly. It performs a basic import test to ensure that TensorFlow, OpenCV, and other dependencies are available.
