# stress-detection-ml
This project uses machine learning to detect stress in delivery agents based on physiological data like heart rate and blood pressure. Using a Random Forest Classifier, it predicts stress levels and offers delivery reassignment suggestions. Perfect for machine learning beginners looking for a practical, real-world application.
# Agent Stress Detection Using Random Forest

**Smart stress monitoring for smarter logistics.**  
This beginner-friendly project helps you understand the complete ML pipeline—from data preprocessing to prediction and visualization—while solving a real-world problem.

## 🧠 About the Project

This project uses physiological data (e.g., heart rate, blood pressure, HRV, etc.) to **detect stress levels** in delivery agents. A Random Forest Classifier is trained to predict whether an agent is stressed based on this data. If an agent is stressed, the system can suggest reassigning the delivery to another agent.

Built with simplicity in mind, this is a great project for **machine learning beginners** looking to understand end-to-end model development, including:

- Data validation and preprocessing
- Model training and evaluation
- User input and CLI prediction
- Visualization and exception handling

## 🗂️ Project Structure

├── stress_detection.py # Main Python script
├── agents_physiological_data.csv # Input CSV file (must be provided)
├── requirements.txt # Dependencies
├── LICENSE # MIT License
└── README.md # Project description and instructions

bash
Copy
Edit

## 📊 Sample Input CSV Format

Make sure your CSV file contains the following columns:

| heart_rate | hrv | systolic_bp | diastolic_bp | body_temp |
|------------|-----|-------------|--------------|-----------|
| 85         | 50  | 125         | 80           | 36.6      |

⚠️ If the file is missing or contains invalid data, the program will handle it gracefully.

## 🛠️ Installation & Setup

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/your-repository-name.git
   cd your-repository-name
Install the required Python libraries:

bash
Copy
Edit
pip install -r requirements.txt
Run the program:

bash
Copy
Edit
python stress_detection.py
🧪 Example CLI Interaction
text
Copy
Edit
Enter the following data for the agent:
Heart Rate (bpm): 110
HRV (ms): 30
Systolic BP (mmHg): 135
Diastolic BP (mmHg): 90
Body Temperature (°C): 37.2

The agent is stressed.
Your delivery is being given to other available agents.
✅ Model Details
Algorithm: Random Forest Classifier

Preprocessing: MinMaxScaler

Performance Metrics: Accuracy, Precision, Recall (via classification report)

📈 Features
Real-time stress classification via CLI

Min-Max normalization of features

Handles missing or invalid values

Visual comparison of true vs predicted labels

Beginner-friendly structure and documentation

