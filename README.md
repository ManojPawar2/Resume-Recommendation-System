# Resume Recommendation System 🧠

This is a **Streamlit-based Resume Recommendation Website** that uses NLP and cosine similarity to:
- Recommend suitable positions based on uploaded resumes.
- Select the most suitable resume for a given job position.

### 🚀 Tech Stack
- **Python**
- **Streamlit**
- **scikit-learn**
- **pdfplumber**
- **Pandas**

### 🧩 How it works
1. Upload a resume (PDF).
2. The system extracts text using `pdfplumber`.
3. Text is vectorized using a pre-trained TF-IDF model (`vectorizer.pkl`).
4. Cosine similarity is computed with pre-stored job role data (`data.pkl`, `feature_matrix.pkl`).
5. The top matching positions or best resume for a position are displayed.

### ▶️ Run locally
```bash
pip install -r requirements.txt
streamlit run web.py
