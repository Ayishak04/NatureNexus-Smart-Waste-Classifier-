<img width="1440" alt="Screenshot 2025-02-25 at 3 43 37 PM" src="https://github.com/user-attachments/assets/e8857158-dfbc-4800-a773-5f300f125ccd" /># SmartWasteClassifier

Smart Waste Management is an AI-powered solution designed to classify waste into organic and recyclable categories. This helps in efficient waste sorting, reducing pollution, and promoting recycling. The system utilizes Azure Custom Vision to analyze images and determine the correct waste category.

✨ Features

AI-Powered Waste Classification – Uses Azure Custom Vision for accurate waste classification.

User-Friendly Interface – Upload images via a simple web interface.

Real-Time Predictions – Get instant results with classification and recycling tips.

Future Scalability – Can be integrated with IoT-based smart bins.

🛠️ Tech Stack

Frontend: HTML, CSS, JavaScript

Backend: Python (Flask)

Cloud Services: Microsoft Azure Custom Vision

Introduction

This guide will help you set up and run the Smart Waste Classification project using your own Azure subscription. If the app shows an error related to an inactive subscription, follow these steps to update the required credentials.

1️⃣ Prerequisites

An active Azure subscription.

Access to Azure Custom Vision (or any trained model for waste classification).

Python installed on your system.

Required dependencies installed (see Step 4).

2️⃣ Get Your Azure Prediction Key & URL

If You Already Have a Trained Model:

Go to Azure Custom Vision.

Sign in and select your Custom Vision project.

Click on Performance (or Predictions) in the left menu.

Click on Prediction URL and copy:

Prediction Key

Prediction URL

Replace these values in app.py:

PREDICTION_KEY = "your_new_prediction_key"
PREDICTION_URL = "your_new_prediction_url"

Save the file.

If You Need to Train a Model:

Create a new project in Azure Custom Vision.

Upload waste classification images and label them.

Click Train to train the model.

Once trained, Publish the model and get the Prediction Key & URL (same steps as above).

Update app.py with these new credentials.

3️⃣ Run the Application

Clone this project or download the files.

Open a terminal in the project folder.

Install required dependencies:

pip install -r requirements.txt

Run the Flask app:

python app.py

Open your browser and go to http://127.0.0.1:5000/ to test the app.

4️⃣ Troubleshooting

Error: No Active Subscription → Ensure you updated PREDICTION_KEY and PREDICTION_URL.

App Not Running? → Check if all dependencies are installed.

Wrong Predictions? → Make sure your Azure model is correctly trained and published.

🎯 Conclusion

By following these steps, you should be able to run the project with your own Azure credentials. If you encounter any issues, verify your Azure setup or contact support.



##Pitch Video

watch our pitch video here-> https://drive.google.com/file/d/1-1QJOJb4Grb2pj3QMQ73OD83OuJffj_d/view?usp=drivesdk


