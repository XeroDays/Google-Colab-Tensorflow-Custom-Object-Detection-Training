# Custom Model Training on Google Colab

This repository provides a step-by-step guide for training a custom object detection model using Google Colab. It includes setting up dependencies, preparing the dataset, and executing the training script.

## Prerequisites

1. Install the required dependencies by running:
   ```bash
   pip install -r requirements.txt
   ```
2. Prepare your dataset by creating a zip file named `MainContent.zip` that includes:
   ```
   MainContent.zip
   ├── Tensorflow/workspace/images/train/  # Contains images and XML label files for training
   ├── Tensorflow/workspace/images/test/   # Contains images and XML label files for testing
   ```
3. Upload `MainContent.zip` to Google Colab before running the training script.

## Steps to Train the Model

### 1. Upload Dataset to Colab
After creating the `MainContent.zip` file, upload it to your Google Colab workspace.

### 2. Testing if everything is working
Run the code blocks one by one until you reach to the code 

    VERIFICATION_SCRIPT = os.path.join(paths['APIMODEL_PATH'], 'research', 'object_detection', 'builders', 'model_builder_tf2_test.py')
    # Verify Installation
    !python {VERIFICATION_SCRIPT}
