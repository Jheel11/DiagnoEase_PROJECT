
# DiagnoEase – AI-Powered Blood Report Summarization & Health Insight System

## 🩺 Project Overview

DiagnoEase is an AI-powered mobile application designed to transform raw medical blood test reports (CBC) into simple, layman-friendly summaries. By combining deep learning and natural language processing, it solves a real-world healthcare challenge: helping non-medical individuals understand their health without needing expert interpretation.

This system eliminates the dependency on constant clinical visits by offering instant, AI-generated interpretations of blood reports, empowering users to stay informed about their health — anytime, anywhere.

---

## 🚀 Why This Matters

Millions of people receive CBC test reports every year but often fail to grasp the meaning of complex medical terms. DiagnoEase bridges this critical gap by:

- Automatically extracting data from PDF reports.
- Generating human-understandable summaries using fine-tuned transformer models.
- Offering fast, on-the-go results through a mobile app.

This innovation makes preventive healthcare more accessible, especially in rural or under-served areas, and reduces unnecessary hospital follow-ups.

---

## 📊 Dataset

- ~10,000 entries combining real CBC PDF reports (anonymized) collected from students and structured .xlsx datasets from Kaggle & Mendeley.
- Extracted parameters include:
  - Hemoglobin, RBC Count, WBC Count, Platelet Count
  - PCV, MCV, MCH, MCHC, RDW
  - Differential Leukocyte Counts, MPV, PCT, PDW
- Each report is paired with a manually written summary including diseases users may be prone to highlighting abnormalities in understandable language.
- Data stored and processed via structured Excel files for training and evaluation.

---

## ⚙️ Methodology

- Data Collection
  - Gathered anonymized medical PDFs and public datasets.
- Preprocessing
  - Extracted values via PyMuPDF, structured them into tabular format.
  - Cleaned and tokenized summaries using NLP techniques.
- Model Training
  - Fine-tuned transformer models (T5, BART) on report-summary pairs.
  - Evaluated using ROUGE metrics and validation loss.
- Deployment
  - Built Flask-based backend API serving the summarization model.
  - Kotlin-based Android app for real-time report upload and feedback.

---



## 💡 Tech Stack

- Frontend (Mobile App): Kotlin (Android Studio)
- Backend API: Python + Flask
- AI Models: HuggingFace Transformers (T5, BART)
- Data Handling: Pandas, NumPy, PyMuPDF
- Preprocessing: NLTK, Scikit-learn
- Model Evaluation: ROUGE (via evaluate library)
- Visualization (for internal testing): Matplotlib, Seaborn

---

## 📱 How It Works

1. Users upload a CBC PDF report via the Kotlin Android app.
2. The app sends the file to a Flask API for processing.
3. AI model extracts values, summarizes the report in plain English.
4. Summary + risk insights are sent back to the app instantly.

---

## 🌐 Real-World Impact

- Reduces patient confusion and anxiety over medical reports.
- Minimizes unnecessary clinic visits for basic report interpretation.
- Boosts accessibility to healthcare knowledge in remote regions.
- Enables doctors to focus on more critical diagnostics while patients stay informed.

---

## 🔭 Future Scope

We are actively working to expand DiagnoEase into a full-fledged health monitoring platform:

- Expanding scope to  summarize all other domains reports and not only specifically CBC 
- Deployment of the app on the Google Play Store.
- Intake of user-specific data (age, gender, medical history).
- Visual dashboards to track CBC trends using graphs and plots.
- Integration of a nutritional/diet recommendation system based on test results.
- High-grade user data privacy and end-to-end encryption for security compliance.

---

## 🙌 Get Involved

We believe this tool can help revolutionize preventive care and health literacy. If you're a healthcare professional, researcher, or developer interested in contributing, feel free to reach out!

Email: jheelturakhia@gmail.com and khushipanchal@gmail.com  


---
