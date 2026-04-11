# Fraud Detection

## Data Source
Here's how to get the data:
1. Open https://www.kaggle.com/datasets/whenamancodes/fraud-detection on browser.
2. Download the data. It comes in forms of a ZIP file.
3. Extract the ZIP file, and you'll get a CSV file named "creditcard."
4. Make a first-level directory named "data" into the project repository.
5. Move the CSV file into the created directory.

## Virtual Environment
Here's how to prepare the virtual environment:
1. Choose the virtual environment of your choice and create one.
2. Install PIP if it doesn't exist at the first place.
3. Make sure you're on the project's home path.
4. Install the packages with this command: `pip install -r requirements.txt`

## Data Preparation
Run the "split_data" notebook located in the "notebooks" directory.

## Notebooks Testing

### MLflow
Here's how to run MLflow:
1. Open the terminal.
2. Check that the port 8080 in the localhost is empty.
3. Enter the "mlflow" directory in this project.
4. Start MLflow with this command: `mlflow server --host 127.0.0.1 --port 8080`
5. Press "Ctrl + C" to stop the server.