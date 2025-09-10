# 🐦 EmpathyBot: TweetEval Emotion + RAG Few-Shot

**EmpathyBot** is a sentiment-aware chatbot pipeline that combines **tweet emotion classification**, **retrieval-augmented generation (RAG)**, and **few-shot prompt engineering**.  
It leverages the [TweetEval](https://huggingface.co/datasets/cardiffnlp/tweet_eval) emotion dataset with a pretrained transformer classifier and an explanation module powered by FAISS and GPT-style generation.

---

## ✨ Key Features
- **Emotion Classification**  
  Uses [`bhadresh-savani/distilbert-base-uncased-emotion`](https://huggingface.co/bhadresh-savani/distilbert-base-uncased-emotion) to classify tweets into 6 emotions:
  - joy
  - sadness
  - anger
  - love
  - surprise
  - fear

- **RAG Explainer**  
  Retrieves semantically similar tweets from a knowledge base (`kb.txt`) using **SentenceTransformers** + **FAISS**.

- **Few-Shot Prompting**  
  Augments the prompt with 3 sampled (tweet, label) pairs to improve explainability.

- **Streamlit App**  
  Interactive UI that displays:
  - predicted emotion
  - generated explanation
  - retrieved supporting tweets

- **Colab-Friendly**  
  Works end-to-end on free Colab, with ngrok providing a public URL to the Streamlit app.

---

Google Drive for Demo and project : 
https://drive.google.com/drive/folders/1vYs0hOo5KnF03tiJ6eyo-s_fKOg5N-Hk?usp=sharing

note-book link : 
https://colab.research.google.com/drive/1bT0oCt29tIK4lyucIY9lhrx1-FYeQEL9?usp=sharing
