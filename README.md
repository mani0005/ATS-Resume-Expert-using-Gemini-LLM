# 🧠 ATS Resume Expert using Gemini LLM

An **AI-powered Applicant Tracking System (ATS)** built with **Streamlit** and **Google’s Gemini LLM**, designed to evaluate resumes against job descriptions.  
It provides **ATS score percentages**, identifies **missing keywords**, and offers **HR-style feedback** — helping candidates improve their resumes and recruiters make better shortlisting decisions.

---

## 🚀 Features

- 📄 **Upload Resume (PDF)** and analyze it instantly.  
- 🧠 **Gemini LLM-powered evaluation** for intelligent, context-aware analysis.  
- 🎯 **ATS-style match percentage** with missing keywords and feedback.  
- 👩‍💼 **HR-style qualitative review** highlighting strengths and weaknesses.  
- 🌐 Simple, interactive **Streamlit web interface**.

---

## 🧩 Tech Stack

| Component | Technology |
|------------|-------------|
| **Frontend / UI** | Streamlit |
| **Backend** | Python |
| **AI Model** | Google Gemini (Generative AI) |
| **PDF Processing** | pdf2image, Pillow |
| **Environment Management** | python-dotenv |

---

## 📁 Project Structure

ATS-Resume-Expert/
│
├── app.py # Main Streamlit app
├── requirements.txt # Python dependencies
├── .env # Contains your Google API key (not uploaded)
└── README.md # Project documentation

---

## Requirements
streamlit
google-generativeai
python-dotenv
pdf2image

---

## How It Works

1. User enters a job description.
2. Uploads a resume (PDF).
3. The app converts the first page of the PDF into an image using pdf2image.
4. Sends both the job description and resume image to Google Gemini LLM.
5. The LLM returns:
   -HR-style evaluation
   -ATS match percentage
   -Missing keywords and improvement tips

---

### Required terminal prompts:
(Download the latest version of anaconda)
>>conda create -p venv python==3.10 -y
>>conda activate venv/
>>pip install -r requirements.txt
get your google_api_key from (https://aistudio.google.com/)
## RUN THE APPLICATION USING:
streamlit run app.py

---

## Troubleshooting
**pdf2image not working?**
Install Poppler (required by pdf2image):
>>Windows: Download from Poppler for Windows
>>macOS: brew install poppler
>>Linux: sudo apt-get install poppler-utils


## CLONE
```bash
>>git clone https://github.com/mani0005/ATS-Resume-Expert.git
>>cd ATS-Resume-Expert
