# 📰 July 2024 Movement Twitter News Summarization

A project focusing on abstractive summarization of tweets related to the **July Revolution 2024 in Bangladesh**, using state-of-the-art transformer-based models like **BART**, **T5**, and **PEGASUS**.

## ✨ Abstract

Twitter serves as a critical real-time news source, especially during socio-political events. During the July Revolution 2024, a vast number of user-generated tweets presented fragmented yet valuable information. This project summarizes such tweets using NLP techniques to reduce information overload and highlight the key events.

I applied **abstractive summarization** using three transformer models and evaluated them using **ROUGE** and **BERTScore** metrics. Among the models, **BART** achieved the best performance in terms of both lexical and semantic similarity.

---

## 📊 Project Highlights

- ✅ Collected 600+ tweets using Twitter API and manual scraping  
- 🧹 Preprocessed tweets (lowercasing, noise removal, lemmatization, etc.)
- 🤖 Summarized tweets using:
  - **BART**
  - **T5**
  - **PEGASUS**
- 📏 Evaluated using:
  - **ROUGE-1**, **ROUGE-2**, **ROUGE-L**
  - **BERTScore**

---

## 🛠️ Technologies Used

- Python 🐍
- Hugging Face Transformers 🤗
- Pandas, NumPy, Matplotlib
- ROUGE and BERTScore libraries

---

## 📁 Dataset

- Total Tweets: ~600  
- Source: Twitter (API + manual collection)  
- Format: CSV  
- Fields:
  - `tweetID` — unique ID
  - `tweets` — tweet content

Hashtags used for filtering:  
`#JulyRevolutionBangladesh`, `#BangladeshProtests`, `#36july`

---

## 🧪 Methodology

1. **Data Preprocessing**  
   - Lowercasing  
   - URL, mentions, hashtag, punctuation, digit removal  
   - Stopword removal  
   - Lemmatization  
   - Whitespace normalization

2. **Modeling**  
   Applied three transformer-based models:
   - BART
   - T5
   - PEGASUS

3. **Evaluation**  
   - ROUGE (1, 2, L) for lexical overlap  
   - BERTScore for semantic alignment

---

## 📈 Results

| Model   | ROUGE-1 | ROUGE-2 | ROUGE-L | BERTScore F1 |
|---------|----------|----------|----------|----------------|
| **BART**    | 0.6191   | 0.3843   | 0.5487   | **0.9144**     |
| T5      | 0.5726   | 0.3539   | 0.5015   | 0.9017         |
| Pegasus | 0.1854   | 0.0393   | 0.1278   | 0.8530         |

📌 **BART** produced the most accurate, coherent, and context-aware summaries.

---



## 🔮 Future Work

- Expand the dataset size and diversity  
- Fine-tune models on domain-specific (Bengali + social media) data  
- Integrate hybrid summarization (abstractive + extractive)  
- Use sentiment and NER for deeper summarization

---

## 📜 License

This project is for academic and research purposes only.

---



