🏠 Housing Price Prediction System :

A complete Machine Learning project that predicts housing prices using structured data. This project demonstrates an end-to-end ML pipeline including data preprocessing, model training, evaluation, and inference.

📌 Project Overview :

This project aims to predict the median house value based on various features such as income, location, and housing characteristics. It uses a Random Forest Regressor along with a robust preprocessing pipeline.

🚀 Features :

• 📊 Data preprocessing using Pipeline and ColumnTransformer

• 🔍 Stratified sampling for balanced dataset splitting

• ⚙️ Automatic model training & saving

• 🔁 Reusable pipeline for inference

• 📈 Model prediction saved to CSV

• 🧠 Multiple models tested (Linear Regression, Decision Tree, Random Forest)

🗂️ Project Structure :


├── housing.csv          # Original dataset

├── input.csv            # Test input data

├── output.csv           # Predictions output

├── model.pkl            # Trained ML model

├── pipline.pkl          # Data preprocessing pipeline

├── main.py              # Main execution script (train + inference)

├── main_old.py          # Model comparison & evaluation

└── README.md            # Project documentation

🛠️ Technologies Used :

  • Python 🐍
  
  • Pandas
  
  • NumPy
  
  • Scikit-learn
  
  • Joblib

⚙️ Installation :

Clone the repository:

</> Bash
git clone https://github.com/shiyalkishan/housing_price_prediction_project.git

cd housing_price_prediction_project

Install dependencies:

</> Bash
pip install -r requirements.txt

Or manually:

</> Bash
pip install pandas numpy scikit-learn joblib

▶️ How to Run :

🔹 Step 1: Train Model (First Run)

</> Bash
python main.py

• Reads housing.csv
• Splits data using stratified sampling
• Trains Random Forest model
• Saves:
  • model.pkl
  • pipline.pkl

🔹Step 2: Run Inference

</> Bash
python main.py

- Loads saved model & pipeline
- Reads input.csv
- Predicts house prices
- Saves results to output.csv

🧠 ML Pipeline Explanation :

🔸 Numerical Data Processing:
  - Missing values → Median Imputation
  - Feature scaling → StandardScaler
🔸 Categorical Data Processing:
  - One-hot encoding for ocean_proximity
🔸 Model Used:
  -🌲 Random Forest Regressor (final model)

📊 Model Evaluation (from main_old.py)

The project compares:
- Linear Regression
- Decision Tree
- Random Forest
Using:
- Cross-validation (CV = 10)
- RMSE (Root Mean Squared Error)

📈 Sample Output
Feature Inputs	    Predicted Price
Sample Row	        ₹XXX,XXX

(Output stored in output.csv)

🔮 Future Improvements
- Hyperparameter tuning (GridSearchCV)
- Model deployment (Flask / FastAPI)
- Add visualization dashboard
- Use advanced models (XGBoost, LightGBM)
🤝 Contributing

Pull requests are welcome. For major changes, please open an issue first.

📜 License

This project is open-source and available under the MIT License.

👨‍💻 Author

Kishan Shiyal

⭐ Support

If you like this project, give it a ⭐ on GitHub!
