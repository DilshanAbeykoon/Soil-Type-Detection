# Soil Type Predictor

This project aims to predict the type of soil (Black Soil, Cinder Soil, Laterite Soil, Peat Soil, Yellow Soil) based on input images using a deep learning model.

## Overview

The project consists of the following components:

1. **Data Preparation**: Images of different soil types are collected and organized into appropriate directories.

2. **Model Training**: A Convolutional Neural Network (CNN) model is trained on the collected images using TensorFlow and Keras.

3. **Model Evaluation**: The trained model is evaluated using validation data to assess its performance.

4. **Model Deployment**: Two deployment options are provided:
    - **Google Colab**: A notebook is included demonstrating how to train, evaluate, and deploy the model using Google Colab.
    - **Flask Web App**: A Flask web application is provided for deploying the model as a REST API.

## Usage

### Training the Model
- To train the model, run the provided notebook `Soil_Type_Prediction.ipynb` in Google Colab.
- Ensure the data is organized in appropriate directories (`Black Soil`, `Cinder Soil`, `Laterite Soil`, `Peat Soil`, `Yellow Soil`).
- Adjust hyperparameters such as batch size, epochs, and model architecture as needed.

### Deploying the Model as a REST API
- Install the required dependencies by running `pip install -r requirements.txt`.
- Run the Flask application using `python app.py`.
- Send POST requests to `http://localhost:5000/predict` with input images to get predictions.

### Model Evaluation
- Evaluate the model's performance using the provided notebook or script `evaluate_model.py`.

## File Structure
├── data/

│ ├── Black Soil/

│ ├── Cinder Soil/

│ ├── Laterite Soil/

│ ├── Peat Soil/

│ └── Yellow Soil/

├── models/

│ └── soil_classification_model.h5

├── app.py

├── evaluate_model.py

├── requirements.txt

├── Soil_Type_Prediction.ipynb

└── README.md


## Dependencies

- Python 3.x
- TensorFlow
- Keras
- Flask

## Contributing

Contributions are welcome! Please feel free to open issues or pull requests for any improvements or new features.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

