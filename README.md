# Grant Recommender for Startup Founders

This is a machine learning–powered recommendation system designed to help startup founders discover relevant public funding opportunities, using semantic search over California state grant data.

## 🔧 Project Structure

```
grant-recommender/
├── app.py                    # Streamlit web app for user interaction
├── build_index.py           # Script to generate vector index from grant data
├── requirements.txt         # List of Python dependencies
├── data/
│   └── california_grants.json       # Source data (place your JSON here)
├── model/
│   ├── grant_vectors.npy
│   ├── grant_ids.txt
│   └── grant_index.faiss
├── docs/
│   └── Grant_Recommender_Report.docx
```

## 🚀 Quickstart

### 1. Install dependencies

```bash
pip install -r requirements.txt
```

### 2. Add your grant data

Place your exported `california_grants.json` inside the `data/` directory.

### 3. Build vector index

```bash
python build_index.py
```

### 4. Launch the app

```bash
streamlit run app.py
```

## 📂 Deliverables

- `build_index.py`: Turns grant descriptions into semantic vectors using Sentence-BERT
- `app.py`: Streamlit UI for user input and real-time recommendations
- `requirements.txt`: Required Python packages
- `Grant_Recommender_Report.docx`: Final report detailing system architecture and usage

## 📌 Next Steps (for expansion)

- Add metadata display for each grant
- Filter by category, deadline, or eligibility
- Deploy to cloud (e.g., Streamlit Cloud or AWS EC2)

---

**Maintained by [Your Name] — For demonstration and mentorship use**
