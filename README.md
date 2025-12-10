# Keyword Extraction – Navigating the Data Labyrinth

This project is a TF-IDF based keyword extraction web application built using Python, Scikit-learn, and FastAPI.  
It identifies the most relevant keywords from a given text to support faster and more meaningful information retrieval.

---

## Features
- Automatically extracts top important keywords
- TF-IDF based NLP method
- Stopword removal and preprocessing
- Web interface for user input and result display
- Supports summarization and content analysis use cases

---

## TF-IDF Overview
TF-IDF stands for Term Frequency – Inverse Document Frequency.

It assigns importance scores to words by evaluating:
1. How frequently a word appears in a document (TF)
2. How rare the word is across documents (IDF)

This highlights meaningful words while reducing the influence of very common ones.

---

## Technologies Used

| Category | Tools |
|---------|------|
| Backend | Python, FastAPI |
| NLP & ML | Scikit-learn (TF-IDF Vectorizer) |
| Frontend | HTML, CSS, JavaScript |
| Server & Tools | Uvicorn, Pydantic |

---

## Workflow
1. User inputs text into the web page  
2. Text is cleaned and stopwords are removed  
3. TF-IDF calculates importance of each word  
4. Top-scoring keywords are returned as output

---

## Dataset & Methodology
- Sample text documents were used for testing output accuracy
- TF-IDF vectorization weights words according to importance
- Highest-weighted words are selected as keywords

---

## How to Run the Project Locally

```bash
# Clone the repository
git clone https://github.com/jaqueen1116/Keyword-Extraction-System.git

# Navigate to project folder
cd Keyword-Extraction-System

# Install required packages
pip install -r requirements.txt

# Run the backend server
uvicorn app:app --reload
