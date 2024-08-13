Overview
The Shrimp Farming Forecast Dashboard is designed to predict various metrics such as survival rate, average body weight, biomass, and revenue based on input parameters reflecting the conditions and management of a shrimp farming operation.

Prerequisites
Before you start, ensure you have the following installed:

Python 3.6 or newer
pip (Python package installer)
Installation
1. Set up a Python Environment
It's recommended to use a virtual environment to manage the dependencies separately from your global Python environment.

Create a Virtual Environment
bash
Copy code
python -m venv shrimp_env
Activate the Virtual Environment
On Windows:
bash
Copy code
shrimp_env\Scripts\activate
On macOS and Linux:
bash
Copy code
source shrimp_env/bin/activate
2. Install Required Packages
Install all required packages using pip. Navigate to the project directory where the requirements.txt file is located and run:

bash
Copy code
pip install -r requirements.txt
If you do not have a requirements.txt, install the required packages directly:

bash
Copy code
pip install dash numpy plotly joblib
Usage
Running the Dashboard
To start the dashboard, navigate to the directory containing the dashboard script (app.py) and run:

bash
Copy code
python app.py
This command will start the local server and host your dashboard.

Accessing the Dashboard
Once the server is running, open a web browser and visit:

arduino
Copy code
http://127.0.0.1:8050/
This URL will direct you to the locally hosted dashboard where you can interact with the visualization and input fields.

Dashboard Features
Input Fields: Users can input various parameters that affect shrimp growth and farm conditions, such as total seed, area, total shrimp, temperatures, salinity, and more.
Graphical Outputs: The dashboard displays:
Survival Rate Over Time
Average Body Weight Over Time
Cumulative Biomass Over Time
Cumulative Revenue Over Time (in IDR)
Model Predictions
The dashboard utilizes machine learning models loaded via joblib to predict the metrics based on input values. Make sure the models (model_sr.pkl and model_abw.pkl) are located in the correct path or update the script to point to the correct location.

Update Predictions
To generate new predictions, adjust the input parameters and click the "Submit" button. The graphs will update based on the new input data.

Troubleshooting
If you encounter issues, ensure that:

All Python packages are installed correctly.
The virtual environment is activated.
The models are loaded without errors. Check the console for any error messages that might indicate what went wrong.
