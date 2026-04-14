# IMDB Sentiment Analysis Streamlit App

[Live Demo](https://imdbrnn-gourav.streamlit.app)

This repository contains a Streamlit app for IMDB sentiment analysis using a simple RNN model.

## Files

- `main.py` — Streamlit app entrypoint
- `simple_rnn_imdb.h5` — saved model weights file
- `requirements.txt` — Python dependencies
- `prediction.ipynb` — notebook for prediction/testing
- `simplernn.ipynb` — notebook for model training
- `embedding.ipynb` — embedding exploration notebook

## Local setup

1. Open PowerShell in this folder:
   ```powershell
   cd C:\Users\goura\OneDrive\Desktop\IMDB_RNN
   ```

2. Activate the virtual environment:
   ```powershell
   & .\.venv\Scripts\Activate.ps1
   ```

3. Install dependencies:
   ```powershell
   pip install -r requirements.txt
   ```

4. Run the Streamlit app locally:
   ```powershell
   streamlit run main.py
   ```

5. The browser should open automatically, or visit the URL shown in the terminal, typically `http://localhost:8501`.

## Deploy to Streamlit Cloud

1. Push the repo to GitHub.
2. Go to https://streamlit.io/cloud.
3. Sign in with GitHub.
4. Click **New app**.
5. Select your repo and the branch.
6. Set the app file to `main.py`.
7. Click **Deploy**.

Streamlit Cloud installs dependencies from `requirements.txt` automatically.

## Notes

- Keep `main.py` and `simple_rnn_imdb.h5` in the same folder.
- If the full model archive fails to load, `main.py` falls back to loading weights only.
- The app uses the IMDB word index and text preprocessing consistent with the model.
