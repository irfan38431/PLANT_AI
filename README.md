# PLANT-AI: Recognition of Plant Diseases by Leaf Image Classification


## Description

Ensuring food security for billions of people requires minimizing crop damage through the timely detection of plant diseases. Developing effective methods for plant disease detection serves the dual purpose of increasing crop yield and reducing unnecessary pesticide use. Traditional methods of disease detection rely on manual examination by farmers or experts, which can be time-consuming and costly, making it impractical for millions of small and medium-sized farms worldwide.

This project presents a plant disease recognition model based on leaf image classification using deep convolutional networks. The model is capable of recognizing 38 different types of plant diseases across 14 different plants and can distinguish plant leaves from their surroundings.

## Leaf Image Classification

This section outlines the process of building a model capable of detecting diseases associated with leaf images. The key steps include:

### 1. Data Gathering

- The dataset used is the **"New Plant Diseases Dataset"**, which can be downloaded from [Kaggle](https://www.kaggle.com/vipoooool/new-plant-diseases-dataset).
- This image dataset contains images of both healthy and unhealthy crop leaves.

### 2. Model Building

- The model was built using PyTorch and includes three different approaches:
  1. A CNN model with Convolutional Layers, Max Pooling, Flattening, and Linear Layers.
  2. Transfer learning using the VGG16 architecture.
  3. Transfer learning using the ResNet34 architecture.

### 3. Training

- The model was trained by experimenting with different variants of the layers mentioned above and by varying hyperparameters.
- The best model achieved a test accuracy of 98.42%.

### 4. Testing

- The model was tested on a total of 17,572 images across 38 classes.
- The model has been used to predict the class of sample images successfully.

### 5. Model Architectures and Results

- Various model architectures were tried, with different learning rates, optimizers, and accuracy results.
- All code versions and results can be seen on [Jovian.ml](https://jovian.ml/soumyajit4419/course-project-plant-disease-classification).

## Details about the Model

- The model is capable of detecting `38` types of `diseases` in `14 unique plants`.
- A detailed list of plants and diseases can be found in the [List](Src).

## Future Work

- Implementing image localization to pinpoint the exact position of the affected leaf area.
- Developing a recommender system to suggest appropriate pesticides and control methods for the detected diseases.
- Implementing management strategies such as fungicide and pesticide applications to provide early information on crop health and disease detection, thereby improving productivity.

## Usage

- **Flask**: Contains code for the Flask server and deployment.
- **TestImages**: Contains sample images for model testing.
- **Src**: Contains all source code for building models.
- **Models**: Contains all pretrained models in PyTorch.

## License

This project is licensed under the MIT License.

## Explanation

For a detailed explanation of the code, refer to the [Medium article](https://medium.com/@soumyajit4419/plant-ai-c8fc95ed90e6?source=friends_link&sk=4707825cbaefa2dcaaa92d0e3ed5de01).
