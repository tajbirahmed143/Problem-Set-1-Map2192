# Problem-set-1-map2192
## README for ProblemSet1.ipynb

This Jupyter Notebook, titled ProblemSet1.ipynb, was generated using Colaboratory and contains Python code for working with the MNIST dataset and training a random walk model. Below, we provide an overview of the code, its purpose, and how to use it.

### Table of Contents
- [Introduction](#introduction)
- [Dependencies](#dependencies)
- [Loading MNIST Dataset](#loading-mnist-dataset)
- [Random Walk Model](#random-walk-model)
- [Training the Model](#training-the-model)
- [Conclusion](#conclusion)

### Introduction
This notebook demonstrates the following tasks:

- Loading the MNIST dataset and displaying a montage of sample images.
- Running a random walk model on the MNIST dataset.
- Training the random walk model to achieve at least 75% accuracy.

### Dependencies
Before running the code in this notebook, ensure that you have the following dependencies installed:

- Python
- NumPy
- Matplotlib
- PyTorch
- scikit-image (skimage)
- wandb (Weights and Biases, used for tracking experiments)

You can install the required packages using the following command:


### Loading MNIST Dataset
The code begins by loading the MNIST dataset using the PyTorch datasets module. You can uncomment and modify the code to load other datasets such as KMNIST or Fashion MNIST if needed. The dataset is loaded and preprocessed, and a montage of sample images is displayed using the `montage_plot` function.

### Random Walk Model
The code then demonstrates a simple random walk model. It reshapes a single image from the dataset and performs matrix multiplication with a randomly generated weight matrix. The result is stored in the variable `y`. The model's predictions are also displayed.

### Training the Model
Next, the notebook defines a function `GPU` to move data to a GPU (if available) and a function `GPU_data` to create GPU tensors without requiring gradients. The random walk model is trained using a stochastic gradient descent (SGD) approach. The code iterates through multiple steps, updating the model weights and calculating accuracy. The best-performing model and its corresponding accuracy are printed.

### Conclusion
This notebook provides a hands-on introduction to loading and working with image data, running a simple random walk model, and training the model to achieve a specific accuracy threshold. You can modify and extend this code as needed for your experiments or analysis.

For more detailed formatting options in Markdown, you can refer to Markdown guides and cheat sheets available online.
