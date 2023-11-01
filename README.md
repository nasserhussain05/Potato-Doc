# PotatoDoc: AI-Powered Potato Plant Disease Detection

## Introduction

PotatoDoc is a Deep learning model for fast and accurate potato plant disease detection which is designed to help farmers and agriculturists in the early detection of diseases in potato plants. By utilizing advanced deep learning models, it categorizes potato plant images into three classes: "Late Blight," "Healthy," and "Early Blight." With this tool, you can quickly identify potential issues and take the necessary steps to protect your potato crops.

# Getting Started
1. Install Dependencies: Navigate to the project's root directory and install the necessary dependencies using pip.
```bash
pip install -r requirements.txt
```
2. Download Dataset: We've utilized a dataset from Kaggle to train our model. You can download it here. Ensure that you only keep the folders related to potatoes.

3. Train the Model: Open the project in your preferred Python development environment (e.g., Jupyter Notebook, VS Code). In the "training" directory, you'll find a Jupyter Notebook named "potato-disease-training.ipynb." Open this notebook and make sure to update the dataset path in cell #2. Run all the cells one by one to train the model.

4. Save the Model: After training, save the generated model with a version number in the "models" folder. This model will be used for predictions.

5. Running the API: The API is powered by FastAPI. To run the API server, navigate to the "api" folder and execute the following command:

```bash
uvicorn main:app --reload --host 0.0.0.0
The API will now be accessible at http://0.0.0.0:8000.
```
6. Running the Frontend: The PotatoDoc frontend provides an easy-to-use interface for users. To run the frontend, navigate to the "frontend" folder. Copy the .env.example file and rename it as .env. Update the REACT_APP_API_URL variable in the .env file with the correct API URL. Then, run the frontend.

With these steps, you'll have PotatoDoc up and running on your local machine.

## How PotatoDoc Works
PotatoDoc is a user-friendly tool:

Upload Image: Users can upload an image of a potato plant they want to analyze.

Click "Predict": By clicking the "Predict" button, PotatoDoc's deep learning model will classify the image into one of the three categories: "Late Blight," "Healthy," or "Early Blight."

## Libraries Used
Here are the primary libraries used in PotatoDoc:

- [TensorFlow](https://tensorflow.org/)
- [FastAPI](https://fastapi.tiangolo.com/)
- [Uvicorn](https://www.uvicorn.org/)
- [Python-Multipart](https://pypi.org/project/python-multipart/)
- [Pillow](https://python-pillow.org/)
- [Matplotlib](https://matplotlib.org/)
- [NumPy](https://numpy.org/)
- [kaggle](https://www.kaggle.com/arjuntejaswi/plant-village) (Remember to keep only the potato-related folders to streamline the training process.)

## Conclusion

**PotatoDoc** is a powerful AI tool designed to assist farmers in the early detection of diseases in potato plants. By following the steps outlined in this README, you can have PotatoDoc running on your machine and start leveraging its capabilities for a healthier and more productive potato crop.

Enjoy using **PotatoDoc**!


