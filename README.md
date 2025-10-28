# 📈 StockVerse — Intelligent Stock Market Analysis & Prediction System

Empowering smarter investment decisions through Machine Learning and Data-Driven Insights.

🧠 Overview

StockVerse is a powerful machine learning–based project designed to analyze and predict stock market trends using both classification and regression models.
It processes NIFTY 50 historical data to predict:

📉 Whether the stock price will go UP or DOWN

💰 The next day’s closing price

Built with Streamlit, scikit-learn, and Pandas, it provides an intuitive dashboard for visualization and live prediction.

🚀 Features

✅ Dual Machine Learning Models

Logistic Regression → Predicts movement direction (Up/Down)

Linear Regression → Predicts next-day closing price

✅ Streamlit Dashboard

Real-time prediction from user input

Visualized recent stock trends

✅ Data Engineering Pipeline

Cleans and processes raw NIFTY50 data

Handles missing values and scaling

✅ Modular Structure

Separate scripts for training, prediction, and UI

✅ Open for Contribution

Anyone can fork this repo and enhance the features further

🧩 Tech Stack
Component	Technology
Language	Python 3.x
Framework	Streamlit
ML Libraries	scikit-learn, Pandas, NumPy, Joblib
Data Source	NIFTY50 Historical Stock Data
Version Control	Git & GitHub
🗂️ Project Structure
StockVerse/
│
├── data/
│   ├── engineered_stock_data.csv
│   └── engineered_stock_data_sample.csv
│
├── models/
│   ├── logistic_model.pkl
│   └── linear_model.pkl
│
├── src/
│   ├── app.py              # Streamlit dashboard
│   └── model_trainer.py    # Model training script
│
├── requirements.txt
├── README.md
└── .gitignore

⚙️ Installation and Setup
1️⃣ Clone the Repository
git clone https://github.com/<your-username>/StockVerse.git
cd StockVerse

2️⃣ Create and Activate Virtual Environment
python -m venv venv
venv\Scripts\activate        # On Windows
# or
source venv/bin/activate     # On Mac/Linux

3️⃣ Install Dependencies
pip install -r requirements.txt

4️⃣ Train the Models

(If you want to retrain with your dataset)

python src/model_trainer.py

5️⃣ Run the Streamlit App
streamlit run src/app.py

💾 Model Files

After training, models are automatically saved to:

models/logistic_model.pkl
models/linear_model.pkl

🌐 Deployment

You can deploy this project easily using:

Streamlit Cloud

Render

Hugging Face Spaces

Just make sure your folder structure is preserved and your dataset (or sample dataset) is uploaded inside /data.

🧮 Example Predictions
Input Features	Logistic Output	Linear Output
RSI: 48, MA5: 1800, Volatility: 0.5	📈 UP	₹1834.76
RSI: 72, MA5: 420	📉 DOWN	₹409.22
🛠️ Commands Reference
Task	Command
Install dependencies	pip install -r requirements.txt
Run dashboard	streamlit run src/app.py
Train models	python src/model_trainer.py
Push changes	git add . && git commit -m "update" && git push origin main
🤝 Contributing

We welcome all contributions! 🎉
You can fork this repository and modify it to give it a better shape —
add new models, data sources, or improve visualization.

Steps to contribute:

Fork this repo

Create your feature branch

git checkout -b feature/NewFeature


Commit your changes

git commit -m "Added new feature"


Push to branch and open a Pull Request

git push origin feature/NewFeature

💬 Contact

📧 Developer: [Your Name or GitHub Profile]
🌐 GitHub: https://github.com/<your-username>/StockVerse

📄 License: MIT

⭐ If you like this project, give it a star on GitHub and share it with your community!

Let’s make StockVerse smarter together 🚀
