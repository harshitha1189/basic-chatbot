
# 🧠 Simple NLP Chatbot (TF-IDF + Cosine Similarity)

This is a basic chatbot built using **Python**, **NLTK**, and **Scikit-Learn**.
It replies to your questions by comparing your message with a text file (corpus) using **TF-IDF** and **cosine similarity**.

---

## 🚀 Features

* Answers questions based on your text corpus
* Uses TF-IDF vectorization
* Cosine similarity to find the best matching sentence
* Handles greetings like “hi”, “hello”, etc.
* Small chat loop with exit option (“bye”)

---

## 📁 Project Files

```
nlp-chatbot/
│── chatbot.ipynb       → main notebook
│── chatbot.txt         → corpus used by the bot
```

---

## 🔧 How It Works

1. Load and clean text from `chatbot.txt`
2. Tokenize into sentences & words
3. Lemmatize using WordNet
4. Convert sentences into TF-IDF vectors
5. Compare user input with all sentences using cosine similarity
6. Return the closest matching answer

---

## ▶️ How to Run

1. Install requirements:

   ```
   pip install nltk scikit-learn
   ```
2. Run the notebook (`chatbot.ipynb`)
3. Start typing messages in the chat loop

---

## 📌 Notes

* The bot can **only answer** questions that are somehow related to the contents of `chatbot.txt`
* If similarity is low, it replies:
  **“I am sorry! I don’t understand you.”**

---

## 💡 Example Conversation

```
You: hi
BOT: hey

You: what is data science?
BOT: (returns the most similar sentence from the corpus)

You: bye
BOT: Goodbye! Take care <3
```

---


