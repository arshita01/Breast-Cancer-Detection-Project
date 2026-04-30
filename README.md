**Breast Cancer Detection Using Machine Learning**
**📌 Project Overview**

This project is a web-based application that predicts whether a breast tumor is benign or malignant using machine learning. It also provides an estimated cancer stage and recommended number of chemotherapy sessions based on tumor characteristics.

The system is designed for use by healthcare professionals such as oncologists or lab technicians to assist in quick and data-driven decision-making.

**🚀 Features**
🔐 User Authentication (Login system)
📊 Breast Cancer Prediction (Benign / Malignant)
🧬 Cancer Stage Estimation (Stage I – IV)
💉 Chemotherapy Session Recommendation
👤 Support for:
Existing patient data
New patient input form
🌐 Web interface built using Flask
🛠️ Tech Stack
Frontend: HTML, CSS (Flask Templates)
Backend: Python (Flask)
Machine Learning: Scikit-learn (Random Forest Classifier)
Data Handling: Pandas
Model: Trained on breast cancer dataset
**📂 Project Structure**
Breast-Cancer-Prediction-using-machine-learning/
│
├── app.py                  # Main Flask application
├── data.csv                # Dataset used for training
├── templates/              # HTML templates (UI)
│   ├── login.html
│   ├── choose.html
│   ├── new_patient_form.html
│   └── result.html
│
├── static/                 # CSS / assets (if any)
├── README.md               # Project documentation
└── requirements.txt        # Dependencies (if added)
⚙️ How It Works
**1. Data Processing**
Dataset is loaded using Pandas
Unnecessary columns are removed
Target variable (diagnosis) is encoded
**2. Model Training**
Data is split into training and testing sets
A Random Forest Classifier is trained
Model predicts:
0 → Benign
1 → Malignant
**3. Prediction Logic**
User inputs tumor features
Model predicts diagnosis
If malignant:
Cancer stage is estimated based on area_mean
Chemotherapy sessions are recommended
**🧠 Stage & Chemotherapy Logic**
Area Mean Range	Cancer Stage	Chemo Sessions
< 500	Stage I	4
500–1000	Stage II	6
1000–1500	Stage III	8
> 1500	Stage IV	10
🔑 Login Credentials (Default)
**Username: admin**
**Password: password123**
**▶️ How to Run the Project**
Step 1: Clone the Repository
git clone <your-repo-link>
cd Breast-Cancer-Prediction-using-machine-learning
Step 2: Install Dependencies
pip install flask pandas scikit-learn
Step 3: Run the Application
python app.py
Step 4: Open in Browser
http://127.0.0.1:5000/
📊 Dataset
**The dataset contains tumor-related features like:**
Radius
Texture
Perimeter
Area
Smoothness
Used for training the ML model
**🎯 Future Improvements**
🔒 Secure authentication with database (MySQL/MongoDB)
📈 Model accuracy improvement with advanced algorithms
📊 Visualization dashboard (Power BI / Charts)
🧾 Patient report download (PDF)
☁️ Deployment on cloud (AWS / Render / Railway)
