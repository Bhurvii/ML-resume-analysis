# ML-based Resume Analysis & Job Recommendation System

This project is a Flask-based web application that analyzes resumes using Natural Language Processing (NLP) and Machine Learning techniques.  
It categorizes resumes into job domains, recommends suitable job roles, and extracts key information such as contact details, skills, and education.

The project is learning-oriented and focuses on understanding how automated resume screening systems work and their limitations.

---

## Features
- Upload resumes in **PDF or TXT** format
- Resume text cleaning and preprocessing
- Resume categorization using **TF-IDF + Random Forest**
- Job role recommendation using a separate ML model
- Extraction of:
  - Name
  - Email address
  - Phone number
  - Skills
  - Education keywords
- Simple web interface built with Flask

---

## Tech Stack
- Python
- Flask
- Machine Learning (Random Forest)
- Natural Language Processing (NLP)
- TF-IDF Vectorization
- Scikit-learn
- PyPDF2
- Regex-based text parsing

---

## Project Workflow
1. User uploads a resume (PDF or TXT)
2. Resume text is extracted and cleaned
3. Text is vectorized using TF-IDF
4. ML models predict:
   - Resume category
   - Recommended job role
5. Resume details (skills, education, contact info) are extracted using regex
6. Results are displayed on the web interface

---

## Project Structure
- `app.py` – Flask application and ML inference logic
- `models/` – Trained ML models and vectorizers
- `templates/` – HTML templates
- `*.ipynb` – Notebooks used for training and experimentation

---

## Limitations
- Uses predefined skill and education keyword lists
- Dataset size and diversity are limited
- Recommendations are classification-based, not personalized
- Intended as a prototype, not a production hiring system

---

## What I Learned
- Applying NLP preprocessing to real-world resume data
- Using TF-IDF and Random Forest for text classification
- Integrating ML models into a Flask web application
- Understanding ethical and bias-related challenges in automated resume screening

---

## Future Improvements
- Improve dataset quality and diversity
- Add explainability to predictions
- Enhance UI and deploy the application
- Replace rule-based extraction with NLP models
