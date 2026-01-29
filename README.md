# Bangalore Home Price Prediction

This project is an end-to-end Machine Learning application that predicts real estate prices in Bangalore, India. It includes a Python backend server (Flask) and a web frontend, using a Linear Regression model trained on a real-estate dataset.

## 📂 Project Structure

```bash
Bangalore_Home_Price_Prediction/
│
├── artifacts/              # Saved model files
│   ├── bangalore_home_prices_model.pickle
│   └── columns.json
│
├── server/                 # Backend code
│   ├── server.py           # Flask server
│   ├── util.py             # Utility functions (loads artifacts)
│   └── artifacts/          # (Copy of artifacts for server access)
│
├── client/                 # Frontend code (HTML/CSS/JS)
│   ├── app.html
│   ├── app.css
│   └── app.js
│
└── model/                  # Jupyter Notebooks for model training
    └── bangalore_home_prices_final.ipynb

```

## 🛠️ Technologies Used

* **Frontend:** HTML, CSS, JavaScript, jQuery
* **Backend:** Python, Flask
* **Machine Learning:** Scikit-Learn, Pandas, NumPy
* **Deployment:** Nginx (optional), AWS EC2 (optional)

## 🚀 Setup & Installation

To run this project locally, you need to set up the Python environment and install the required dependencies.

### 1. Clone the Repository

```bash
git clone https://github.com/ritesh-1912/Bangalore_Home_Price_Prediction.git
cd Bangalore_Home_Price_Prediction

```

### 2. Create the Environment

It is recommended to use Anaconda to manage the environment.

```bash
conda create --name reg_project python=3.10
conda activate reg_project

```

### 3. Install Dependencies

Install the necessary Python libraries within your environment:

```bash
conda install flask scikit-learn pandas numpy
# OR use pip
pip install flask scikit-learn pandas numpy

```

## 🏃‍♂️ How to Run

### 1. Start the Flask Server

Navigate to the server directory and run the application.

```bash
cd server
python server.py

```

*You should see a message indicating the server is running (usually on port 5000).*

### 2. Launch the Website

1. Go to the `client` folder.
2. Open `app.html` in your web browser (Chrome/Firefox/Safari).
3. The frontend will connect to the backend (check your browser console if there are connection issues).

## 🧠 Model Details

* **Algorithm:** Linear Regression
* **Data Cleaning:** Handling NA values, dimensionality reduction, One Hot Encoding for location.
* **Outlier Removal:** Logic based on square ft per bedroom and standard deviation checks.

## 📄 License

This project is open-source and available under the MIT License.
