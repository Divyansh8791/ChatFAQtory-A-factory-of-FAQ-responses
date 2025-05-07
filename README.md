# 🤖 ChatFAQtory-A-factory-of-FAQ-responses

**ChatFAQtory** is a smart, lightweight chatbot built to instantly answer user queries using a curated FAQ dataset. It leverages sentence embeddings, semantic search with FAISS, and the power of Google's Gemini model to generate helpful and contextual responses.

---

## 🔍 What It Does

- Accepts any natural language query from the user.
- Uses SentenceTransformers (`all-MiniLM-L6-v2`) to convert text to embeddings.
- Searches the most relevant FAQ using FAISS (cosine similarity).
- Sends that FAQ context + user query to Gemini (via LangChain).
- Gemini generates a smart, friendly response.
- Displays the retrieved FAQ snippet along with the final AI-generated answer.

---

## 🛠️ Tech Stack

| Component              | Purpose                                      |
|------------------------|----------------------------------------------|
| `SentenceTransformers` | Convert FAQ entries and user queries into embeddings |
| `FAISS`                | Perform fast and efficient vector search      |
| `LangChain`            | Manages prompt chaining with Gemini           |
| `Gemini-1.5 Flash`     | Generates intelligent and human-like replies  |
| `Gradio`               | Clean and interactive web-based chatbot UI    |
| `Pandas`               | Data handling and preprocessing               |

---

## 🗂️ Dataset

The bot uses a CSV file (`Final_faqs.csv`) containing Frequently Asked Questions.  
Each entry includes:
- **Question**: A typical user query.
- **Answer**: A helpful response.

---

## 💡 Key Features

- 💬 Natural language interface
- ⚡ Lightning-fast semantic search using FAISS
- 🧠 Context-aware answers powered by Gemini
- 🤝 Friendly greetings and smooth UX
- 📄 Shows the FAQ context used in the answer
- 🌐 One-click Gradio shareable link

---

## 📦 How to Run It

### 1. Clone the Repository

```bash
git clone https://github.com/Divyansh8791/faqenius-chatbot.git
cd faqenius-chatbot
```
### 2. install the requirements
```bash
pip install -r requirements.txt
```
### 3. run the app
```bash
python app.py
```

### Structure of project 
```
├── Final_faqs.csv               # Your FAQ dataset
├── app.py                       # Main chatbot code
├── requirements.txt             # Python dependencies
└── README.md                    # This file
```
---
