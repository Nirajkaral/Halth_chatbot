
# 🩺 HealthGuard AI – Your Personal Health Assistant

HealthGuard AI is an AI-powered health assistant built with **Streamlit**, **Google Gemini AI**, and **Machine Learning**.
It helps users analyze their medical reports, chat with an AI health assistant, and predict their health risk using a trained ML model.

---

## 🚀 Features

✅ **AI Health Chat** – Chat with Google Gemini AI or Hugging Face fallback model.
✅ **PDF Medical Report Upload** – Extracts and processes text from uploaded medical reports.
✅ **Disease Risk Prediction** – Predicts diabetes risk based on **Age, BMI, Glucose, and Blood Pressure** using a **Random Forest Classifier**.
✅ **Theme Switcher** – Choose between **Green & White** or **Red & White** themes.
✅ **Downloadable Health Report** – Get a personalized text report with your health insights.
✅ **Interactive UI** – Powered by **Streamlit** with custom styling.

---

## 🛠️ Tech Stack

* **Frontend / UI**: [Streamlit](https://streamlit.io/)
* **AI Models**: [Google Gemini](https://ai.google.dev/), [Hugging Face Transformers](https://huggingface.co/docs/transformers/index)
* **Machine Learning**: [Scikit-learn](https://scikit-learn.org/stable/)
* **Data Handling**: [Pandas](https://pandas.pydata.org/), [PyMuPDF](https://pymupdf.readthedocs.io/en/latest/)
* **Authentication**: [dotenv](https://pypi.org/project/python-dotenv/)

---

## 📂 Project Structure

```
├── app.py                  # Main Streamlit app  
├── diabetes.csv            # Dataset for ML training  
├── requirements.txt        # Python dependencies  
├── .env                    # API keys (Gemini & HuggingFace)  
└── README.md               # Project documentation  
```

---

## ⚙️ Installation & Setup

1. **Clone the repository**

```bash
git clone https://github.com/Nirajkaral/Halth_chatbot
cd healthguard-ai
```

2. **Create a virtual environment**

```bash
python -m venv venv
source venv/bin/activate   # On Mac/Linux
venv\Scripts\activate      # On Windows
```

3. **Install dependencies**

```bash
pip install -r requirements.txt
```

4. **Add your API keys in `.env` file**

```env
API_KEY=your_google_gemini_api_key
HUGGINGFACE_TOKEN=your_huggingface_token
```

5. **Run the app**

```bash
streamlit run app.py
```

---

## 📊 Machine Learning Model

* **Algorithm**: Random Forest Classifier
* **Dataset**: PIMA Diabetes dataset (`diabetes.csv`)
* **Features Used**: Age, BMI, Glucose, Blood Pressure
* **Output**: Health Risk Prediction (High Risk / Low Risk)

You can also view the model’s classification report inside the app.

---

## 📥 Sample Usage

1. Upload your medical report in PDF.
2. Ask any health-related question in the chat.
3. Enter your health parameters (Age, BMI, Glucose, BP).
4. Click **Predict Health Risk** to get your personalized report.
5. Download the report for future reference.


---

## 🛡️ Disclaimer

This app is for **educational purposes only** and should not replace professional medical advice.
Always consult a qualified healthcare provider for medical concerns.

---

## 🤝 Contributing

Contributions are welcome! Please fork the repo and submit a pull request.

---

## 📜 License

MIT License.

