URL and Content-Based Phishing Detection System Using Deep Learning

ABOUT THE PROJECT 

This project is a deep learning-based phishing detection system designed to identify potentially malicious websites by analysing URL and website-related features.

The system uses a Feed-Forward Neural Network (FNN) to classify submitted URLs as either legitimate or phishing. It combines a trained machine learning model with a web interface that allows users to submit URLs and view the classification results.

The project was developed as my final-year Computer Science project to explore the application of deep learning to cybersecurity, particularly the detection of phishing websites.


✨ Key Features

- Phishing Detection: Classifies submitted URLs as phishing or legitimate.
- Deep Learning Model: Uses a Feed-Forward Neural Network for classification.
- Feature Extraction: Extracts and processes website-related features for model prediction.
- Web Interface: Provides a simple interface for submitting URLs and viewing results.
- Confidence Score: Displays the model's confidence in its prediction.
- Result Logging: Uses Firebase Realtime Database to store classification results and associated timestamps.

Model and Methodology

The system uses a Feed-Forward Neural Network (FNN) Model, a type of artificial neural network in which information moves through the network from the input layer, through one or more hidden layers, to the output layer.


🛠️ Technologies Used 
Python - Core programming language
TensorFlow / Keras - Building and training the neural network
Pandas - Dataset manipulation and analysis
NumPy - Numerical computations
Scikit-learn - Data preprocessing, feature scaling, and model evaluation
Google Colab - Model development and training environment
FastAPI - Backend API for handling prediction requests
HTML - Frontend page structure
JavaScript - Frontend interactions and API communication
Firebase Realtime Database - Storing detection logs and timestamps
Localtunnel - Exposing the development API for external access

📁 Model Files

The trained model and preprocessing artefacts include:

- "fnn_phishing_model.h5" — Saved neural network model.
- "scaler.pkl" — Saved feature-scaling object used during preprocessing.

These files must be loaded correctly during inference, using the same feature order and preprocessing steps applied during training.

🚀 Running the Project

The original development environment uses Google Colab for the model and backend, with Localtunnel providing external access to the API.

To run the project, you will need the project source files, the trained model, the saved scaler, and the required Python dependencies.

The general workflow is:

1. Open the backend or model notebook in Google Colab.
2. Install or import the required dependencies.
3. Load the trained model and saved scaler.
4. Start the FastAPI application.
5. Expose the backend using the configured Localtunnel setup, where required.
6. Open the frontend and configure it to communicate with the backend API.
7. Submit a URL to view its classification result.

The exact commands and configuration depend on the files included in the repository. Firebase credentials and other secrets should be configured securely rather than committed to GitHub.

Limitations

- Predictions depend on the quality and representativeness of the training dataset.
- The model's predictions are not guaranteed to be correct for every URL.
- Confidence scores should not be interpreted as proof that a website is safe or malicious.
- The system should be treated as a decision-support tool rather than a replacement for comprehensive security analysis.
- Detection performance may vary when the system encounters websites or phishing techniques not adequately represented in the training data.

Future Improvements

Potential improvements include:

- Expanding the dataset with more diverse and recent phishing samples.
- Improving feature extraction and selection.
- Comparing the FNN with other machine learning and deep learning approaches.
- Improving the frontend and user experience.
- Strengthening API security and deployment reliability.
- Evaluating the model against additional unseen datasets.

👩🏽‍💻 Author

Oshamo Feyishola Naomi 

Computer Science Graduate | ISC2 Certified in Cybersecurity (CC) 

‼️Disclaimer

This project was developed for academic and educational purposes as part of a final-year Computer Science project. It is intended to support phishing awareness and research into automated website classification.

The system should not be used as the sole basis for determining whether a website is safe.
