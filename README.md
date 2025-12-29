Project: Laptop Price Prediction using Machine Learning
📌 Overview
This end-to-end ML project predicts the price of laptops in Euros based on their specifications. It demonstrates the full ML lifecycle — from data collection to deployment — and integrates a clean Streamlit interface for real-time price prediction.

🚀 Project Workflow
1️⃣ Data Collection

Used a comprehensive laptop dataset containing attributes like Company, Product, CPU, GPU, RAM, Storage, and Display details.

2️⃣ Data Cleaning

Removed null values, handled inconsistent formats, and standardized units (e.g., GHz, GB).

Extracted screen dimensions and display types for better model interpretability.

3️⃣ Feature Engineering

Derived meaningful variables such as CPU_company, GPU_company, Touchscreen, RetinaDisplay, etc.

Selected key predictive features: ['Product', 'CPU_model', 'GPU_model', 'Ram', 'CPU_freq', 'PrimaryStorage', 'TypeName']

4️⃣ Target Encoding

Applied Target Encoding on categorical columns using mean target mapping technique: Each category replaced by the average Price_euros for that category.

5️⃣ Scaling

Used RobustScaler to scale numerical features and minimize outlier influence.

6️⃣ Model Training & Evaluation

Trained Logistic Regression model for regression-based price prediction.

Evaluated model performance using metrics like MAE, RMSE, and R² Score.

7️⃣ Model Deployment

Deployed an interactive Streamlit web app where users input specs (CPU, GPU, RAM, etc.) and get an instant price prediction.

Ensured smooth feature alignment with trained model through preprocessing pipeline.

🖥️ Tech Stack

Language: Python

Libraries: Pandas, NumPy, Scikit-learn, Streamlit, Joblib

Deployment: Streamlit Cloud / Localhost

Encoding & Scaling: Target Encoding, RobustScaler

💡 Key Learnings
Implementing custom target encoding mappings for categorical features.

Building preprocessing pipelines for real-world ML deployment.

Handling feature mismatch errors between training and inference.

Deploying ML models using Streamlit with real-time predictions.

🧩 How to Run Locally
# Clone the repository

git clone 

# Install dependencies

pip install -r requirements.txt

# Run Streamlit app

streamlit run app.py
💻 Streamlit Interface
Users enter laptop configurations → Backend applies encoding/scaling → Model predicts price in Euros.

📎 Author
Onkar Patil Machine Learning Engineer | Data Science Enthusiast 📧 Contact: [[www.linkedin.com/in/opatil345/]]
