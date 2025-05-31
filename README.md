# 💼 Salary Prediction Web App

This is a simple machine learning-based web application that predicts an employee's salary based on:

- Years of experience  
- Test score (out of 10)  
- Interview score (out of 10)

Built using **Flask**, with the model trained using **scikit-learn**, and deployed on **Render**.

🔗 **Live App**: [https://salary-predict-heroku.onrender.com/](https://salary-predict-heroku.onrender.com/)

---

## 📂 Project Structure

```
Salary-Predict-Heroku/
├── model.pkl               # Trained Linear Regression model
├── app.py                  # Flask backend
├── templates/
│   └── index.html          # HTML frontend
├── static/                 # (Optional) Static files like images or stylesheets
├── requirements.txt        # Python dependencies
└── README.md               # Project documentation
```

---

## ⚙️ How It Works

1. User enters values for experience, test score, and interview score.
2. The Flask app sends the input to the machine learning model.
3. The model returns a predicted salary.
4. The result is displayed on the same page.

---

## 🚀 Deployment

The app is deployed on **Render** at:  
👉 [https://salary-predict-heroku.onrender.com/](https://salary-predict-heroku.onrender.com/)

To deploy your own version on Render:

1. Fork this repository.
2. Create a new web service on [Render](https://render.com/).
3. Connect your GitHub repo.
4. Set the start command to:

   ```bash
   gunicorn app:app
   ```

5. Add Python environment:
   - Runtime: `python`
   - Build Command: `pip install -r requirements.txt`
   - Auto-deploy from GitHub (optional)

---

## 🧪 Local Setup

1. **Clone the repo**  
   ```bash
   git clone https://github.com/shreeyanshm/Salary-Predict-Heroku.git
   cd Salary-Predict-Heroku
   ```

2. **Create a virtual environment** (optional but recommended)  
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install dependencies**  
   ```bash
   pip install -r requirements.txt
   ```

4. **Run the app**  
   ```bash
   python app.py
   ```

5. **Visit in browser**  
   Go to [http://127.0.0.1:5000](http://127.0.0.1:5000)

---

## 🧠 Model Info

- Model: **Linear Regression**
- Trained using: `scikit-learn`
- Features:
  - Experience (numeric)
  - Test score (0–10)
  - Interview score (0–10)

---

## 📦 Requirements

Check `requirements.txt` for the full list. Main dependencies include:

- Flask
- scikit-learn
- numpy
- pandas
- gunicorn (for deployment)

---

