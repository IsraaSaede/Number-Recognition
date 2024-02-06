# Number Recognition with Convolutional Neural Network

This project utilizes a Convolutional Neural Network (CNN) to recognize handwritten digits. It includes a graphical user interface (GUI) where users can draw a digit, and the model will predict the digit drawn along with the confidence score.

## Requirements

- Python 3.x
- Libraries:
  - Keras
  - tkinter
  - numpy
  - pandas
  - matplotlib
  - seaborn
  - Pillow
  - win32gui
  - tensorflow (for one-hot encoding)

## Usage

1. Clone the repository to your local machine:git clone <https://github.com/IsraaSaede/Number-Recognition.git>
2. Install the required dependencies:pip install -r requirements.txt
3. Run the application:python <Number-Recognition>.ipynb
4. Draw a digit on the GUI canvas.
5. Click the "Recognize" button to see the predicted digit and confidence score.
6. Click the "Clear" button to clear the canvas and draw a new digit.

## Model Training

The model is trained using the MNIST dataset, which is loaded directly from the Keras library. The training process involves:

- Data preprocessing: Normalizing the pixel values and reshaping the data.
- One-hot encoding the labels.
- Creating a CNN model with two convolutional layers followed by a dense layer.
- Compiling the model with categorical crossentropy loss and Adam optimizer.
- Training the model with early stopping to prevent overfitting.

## Model Evaluation

The trained model's accuracy is evaluated on both the training and testing datasets. 

- Train accuracy: 99.81%
- Test accuracy: 98.66%

## File Descriptions

- `Number-Recognition.ipynb`: Jupyter Notebook containing the code for the number recognition project.
- `mnist.h5`: Pre-trained model file.
- `requirements.txt`: Lists all the required dependencies for the project.

## Acknowledgments

- This project is based on the MNIST dataset and utilizes the Keras library for model training and evaluation.
- GUI implementation is done using the tkinter library.
- Special thanks to the contributors of the libraries used in this project.
