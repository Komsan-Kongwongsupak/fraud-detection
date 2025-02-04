# Credit Card Fraud Detection

## 📌 Project Overview
This project focuses on detecting fraudulent credit card transactions using machine learning. It involves data preprocessing, feature engineering, model training, evaluation, and deployment. The system is designed for real-time fraud detection using an API and includes monitoring tools to track model performance over time.

## 🚀 Features
- **Data Preprocessing**: Cleaning, handling missing values, encoding categorical features, and scaling numerical features.
- **Feature Engineering**: Creating new features based on transaction patterns and customer behavior.
- **Machine Learning Models**: Logistic Regression, Random Forest, XGBoost, LightGBM, Autoencoders, and Isolation Forest.
- **Model Evaluation**: Using precision, recall, F1-score, AUC-ROC, and SHAP for interpretability.
- **Real-Time API**: A Flask/FastAPI-based API for fraud detection.
- **Deployment**: Docker containerization and cloud deployment (AWS/GCP/Azure).
- **Model Monitoring**: Tracking performance using Evidently AI, Grafana, and Prometheus.
- **Visualization**: Interactive dashboards with Power BI/Tableau.

---

## 📂 Project Structure
```
credit-card-fraud-detection/
│── data/                  # Datasets (raw and processed)
│── notebooks/             # Jupyter notebooks for analysis and training
│── src/                   # Source code for preprocessing, modeling, and API
│── models/                # Saved models and checkpoints
│── deployment/            # Docker and cloud deployment scripts
│── monitoring/            # Monitoring scripts and dashboards
│── dashboards/            # Power BI/Tableau dashboards
│── reports/               # Reports and documentation
│── tests/                 # Unit tests for data, model, and API
│── venv/                  # Python virtual environment directory
│── .gitignore             # Git ignore file
│── LICENSE                # License for usage
│── README.md              # Project documentation
```

---

## 🛠️ Installation & Setup
### 1️⃣ Clone the Repository
```sh
git clone https://github.com/your-username/credit-card-fraud-detection.git
cd credit-card-fraud-detection
```

### 2️⃣ Set Up a Virtual Environment
```sh
python -m venv venv
source venv/bin/activate  # On macOS/Linux
venv\Scripts\activate     # On Windows
```

### 3️⃣ Install Dependencies
```sh
pip install -r requirements.txt
```

---

## 🔍 How to Use
### 1️⃣ Train the Model
Run the model training script:
```sh
python src/model_training.py
```
This will train and save the fraud detection model in the `models/` directory.

### 2️⃣ Start the API Server
To deploy the fraud detection model as an API, run:
```sh
python src/fraud_detection_api.py
```
By default, the API runs on `http://127.0.0.1:5000/`.

### 3️⃣ Make a Fraud Detection Request
Use `curl` or Postman to test the API:
```sh
curl -X POST http://127.0.0.1:5000/predict -H "Content-Type: application/json" -d '{
  "TransactionAmount": 200,
  "TransactionLocation": "New York",
  "PaymentMethod": "Credit Card"
}'
```
Response:
```json
{"fraud_prediction": 1}
```

---

## 📊 Model Monitoring & Visualization
- **Model Drift Detection**: Run the Evidently AI monitoring script:
  ```sh
  python monitoring/evidently_monitoring.py
  ```
- **Grafana Dashboard**: Set up real-time fraud detection tracking with Prometheus & Grafana.
- **Power BI/Tableau Dashboards**: Use dashboards in the `dashboards/` folder to visualize transaction patterns.

---

## 📦 Deployment
### 🚀 Using Docker
To containerize the API:
```sh
docker build -t fraud-detection-api .
docker run -p 5000:5000 fraud-detection-api
```

### ☁️ Cloud Deployment
To deploy on AWS/GCP/Azure, follow the scripts in the `deployment/` folder.

---

## ✅ Testing
To run unit tests:
```sh
pytest tests/
```

---

## 📝 License
This project is licensed under the MIT License. See `LICENSE` for details.

---

## 🤝 Contributing
Contributions are welcome! If you’d like to improve the project, submit a pull request.

---

## 📞 Contact
For questions, reach out at: `komsan.kongwongsupak@gmail.com`

