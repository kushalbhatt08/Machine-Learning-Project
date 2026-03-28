# 🤖 Evaluating LLMs for Text Classification & Summarisation

## 📌 Project Overview
This project evaluates the performance of pre-trained Large Language Models (LLMs) 
across two NLP tasks — sentiment classification and abstractive summarisation — using 
real-world datasets from Hugging Face.

The aim is to compare encoder-based and encoder-decoder architectures, analyse their 
strengths and weaknesses, and reflect on fairness, bias, and performance trade-offs. 
This work is part of COMP6012 (Large Language Models and Applications) at Adelaide 
University, 2026.

## 🛠️ Technologies Used
* Python 3.9+
* Jupyter Notebook / Google Colab
* HuggingFace Transformers → LLM model loading & inference
* HuggingFace Datasets → Yelp Reviews & CNN/DailyMail datasets
* Scikit-learn → Classification metrics (Accuracy, F1, Precision, Recall)
* Evaluate & ROUGE Score → Summarisation metrics (ROUGE, BLEU)
* Matplotlib & Seaborn → Results visualisation

## 🔎 Workflow

### 1. Dataset Preparation
   * Loaded Yelp Review Full (650K train / 50K test, 5 classes)
   * Loaded CNN/DailyMail (286K train / 11.5K test pairs)
   * Down-sampled test sets due to GPU constraints
   * Repeated evaluation across multiple random seeds for stable results

### 2. Model Selection & Deployment
   * Loaded pre-trained models via HuggingFace Transformers pipeline
   * Tokenised inputs for each model
   * Run inference on down-sampled test sets

### 3. Evaluation
   * **Classification:** Accuracy, Precision, Recall, F1-Score
   * **Summarisation:** ROUGE-1, ROUGE-2, ROUGE-L, BLEU

## 🧠 Models Used

| Task | Model | Architecture |
|------|-------|--------------|
| Text Classification | `bert-base-uncased` | Encoder-only (BERT) |
| Text Classification | `roberta-base` | Encoder-only (RoBERTa) |
| Text Summarisation | `t5-small` | Encoder-Decoder (T5) |
| Text Summarisation | `facebook/bart-large-cnn` | Encoder-Decoder (BART) |

## 📊 Results & Insights
* RoBERTa outperformed BERT on sentiment classification due to its improved 
  pre-training strategy
* BART-large-cnn produced more fluent and accurate summaries compared to T5-small
* Trade-off: smaller models (T5-small) are faster and cheaper but sacrifice output quality
* Both classification models showed some bias toward majority sentiment classes
* Ensemble of metrics (ROUGE + BLEU) gave a more complete picture of summarisation quality
