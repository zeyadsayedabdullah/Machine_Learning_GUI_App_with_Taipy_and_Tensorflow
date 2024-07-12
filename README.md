# Machine Learning GUI App with Taipy and TensorFlow

This project demonstrates the development of a simple machine learning GUI application using Taipy and TensorFlow. The application allows users to load an image and classify it using a pre-trained neural network model on the CIFAR-10 dataset.

## Project Files

### NeuralNetworkQuickBuilder.ipynb

A Jupyter notebook that contains the steps to quickly build and train a neural network on the CIFAR-10 dataset. The main steps include:

1. **Imports**: Import necessary libraries like Matplotlib, PIL, and NumPy.
2. **Load Dataset**: Load the CIFAR-10 dataset and display the number of training and testing samples.
3. **Map Class Number to Class Name**: Map class indices to their corresponding names (e.g., airplane, automobile).
4. **Plot Samples Along with Their Class Names**: Plot sample images from the dataset along with their class names.
5. **Normalize Samples**: Normalize pixel values of the images.
6. **One Hot Encode Labels**: Convert class labels to one-hot encoded format.
7. **Define Neural Network**: Define the neural network architecture using TensorFlow's Sequential API.
8. **Train Model**: Train the model on the CIFAR-10 training dataset and save the trained model.
9. **Test Model**: Evaluate the model on the CIFAR-10 test dataset and display accuracy.
10. **Fetch Predictions**: Get predictions for test samples and display the predicted and actual class names.

### baseline.keras

The trained model saved from the `NeuralNetworkQuickBuilder.ipynb` notebook.

### classifier.py

A script that creates a GUI application using Taipy to classify images using the trained model. The main components include:

1. **Import Libraries**: Import necessary libraries like Taipy, TensorFlow, PIL, and NumPy.
2. **Load Model**: Load the pre-trained model.
3. **Predict Image**: Define a function to predict the class of a given image.
4. **Create GUI**: Create a simple GUI using Taipy that allows users to upload an image, display the image, and show the predicted class along with the prediction probability.

## Instructions

1. **Clone the repository**:
   ```sh
   git clone <repository_url>
   ```

2. **Install the required packages**:
   ```sh
   pip install -r requirements.txt
   ```

3. **Run the Jupyter notebook** to build and save the model:
   ```sh
   jupyter notebook NeuralNetworkQuickBuilder.ipynb
   ```

4. **Run the classifier.py** to start the GUI application:
   ```sh
   python classifier.py
   ```

5. **Upload an image** using the GUI to classify it.

## Project Structure

```
Machine_Learning_GUI_App_with_Taipy_and_Tensorflow/
├── NeuralNetworkQuickBuilder.ipynb
├── baseline.keras
├── classifier.py
├── requirements.txt
└── README.md
```

## Requirements

- Python 3.7+
- TensorFlow
- Taipy
- Matplotlib
- PIL
- NumPy

Ensure you have all the dependencies installed by using the provided `requirements.txt` file.

## Usage

1. **Build and train the model**: Follow the steps in `NeuralNetworkQuickBuilder.ipynb` to build and train the neural network model on the CIFAR-10 dataset.
2. **Run the GUI application**: Execute `classifier.py` to start the Taipy-based GUI application. Use the application to upload an image and see the classification results.

## Acknowledgements

This project uses the CIFAR-10 dataset, a widely used dataset for machine learning and computer vision research. The dataset is provided by the Canadian Institute for Advanced Research (CIFAR).

watch the video on linkedin https://www.linkedin.com/in/zeyadsayed/
