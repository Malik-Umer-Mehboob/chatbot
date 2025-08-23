
# 📘 Chat with PDF using Gemini

An **AI-powered PDF Chatbot** built with **Streamlit**, **LangChain**, **FAISS**, and **Google Gemini API**.
This project allows users to upload PDF files and ask questions directly from the documents. The system processes the text, creates embeddings, and provides context-aware answers.

---

## 🚀 Features

* Upload multiple PDF files
* Extracts and processes text from PDFs
* Splits text into chunks for better understanding
* Uses **FAISS Vector Database** for similarity search
* Chat with your documents using **Google Gemini (1.5 Flash / Pro)**
* Streamlit-based simple web interface

---

## 📂 Project Structure

```
chat_with_pdf/
│── app.py               # Main Streamlit application
│── .env                 # API key (not shared publicly)
│── faiss_index/         # Local vector DB (auto created after processing)
```

---

## ⚙️ Installation & Setup

### 1. Clone the repository

```bash
git clone <your-repo-url>
cd chat_with_pdf
```

### 2. Create virtual environment

```bash
python -m venv venv
venv\Scripts\activate   # Windows  
source venv/bin/activate   # Mac/Linux  
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Add API Key in `.env`

Create a `.env` file in the project root folder and add:

```
GOOGLE_API_KEY=your_api_key_here
```

You can get your key from 👉 [Google AI Studio](https://aistudio.google.com/apikey)

---

## ▶️ Run the App

```bash
streamlit run app.py
```

Then open browser at → `http://localhost:8501/`

---

## 🖥️ Usage

1. Upload one or more PDF files from the sidebar
2. Click **Submit & Process**
3. Ask any question in the text box
4. Get instant, context-based answers

---

## 📌 Requirements

* Python 3.9+
* Streamlit
* PyPDF2
* LangChain
* FAISS
* Google Generative AI (`google-generativeai`)
* python-dotenv

---

## ⚠️ Common Issues

* **❌ 429 Error (Quota Exceeded):** You are hitting free-tier Gemini API limits. Upgrade your billing plan or use another API key.
* **❌ GOOGLE\_API\_KEY not found:** Make sure `.env` file is in the root folder and properly set.

---

## 🤝 Contribution

Pull requests are welcome. For major changes, please open an issue first.

---

## 📜 License

This project is licensed under the **MIT License**.


