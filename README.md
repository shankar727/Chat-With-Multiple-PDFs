# 📄🤖 AI PDF Chatbot using Gemma 3 (Ollama + Streamlit)

An intelligent PDF Question-Answering system that allows users to upload documents and ask questions in natural language. Powered by Gemma 3 (Ollama) and LangChain, the app retrieves relevant information and responds conversationally.

---

## 🚀 Features

* 📂 Upload multiple PDF files
* 🔍 Extract and process text automatically
* ✂️ Smart text chunking
* 🧠 Context-aware Q&A using LLM
* 💬 Conversational memory (chat history)
* ⚡ Fast local inference with Ollama
* 🎯 Relevant answer retrieval using vector search

---

## 🛠️ Tech Stack

* **Frontend:** Streamlit
* **LLM:** Ollama (Gemma3:4b)
* **Framework:** LangChain
* **Vector Store:** FAISS / Chroma (based on helper)
* **Language:** Python

---

## 📂 Project Structure

```id="f7kq92"
AI-PDF-Chatbot/
│
├── app.py
├── helper.py
├── requirements.txt
└── README.md
```

---

## ⚙️ Installation & Setup

### 1️⃣ Clone the Repository

```bash id="o2lm8a"
git clone https://github.com/your-username/AI-PDF-Chatbot.git
cd AI-PDF-Chatbot
```

---

### 2️⃣ Install Dependencies

```bash id="l9sd1k"
pip install -r requirements.txt
```

---

### 3️⃣ Install Ollama

Download from 👉 https://ollama.com/

Then pull the model:

```bash id="u8hd4p"
ollama pull gemma3:4b
```

---

### 4️⃣ Run the App

```bash id="x3d9qp"
streamlit run app.py
```

App will open in browser automatically.

---

## 🧠 How It Works

1. 📥 User uploads PDF files
2. 📄 Text is extracted using `get_pdf_text()`
3. ✂️ Text is split into chunks (`get_text_chunks()`)
4. 📦 Vector embeddings are created (`get_vector_store()`)
5. 🔎 Retriever finds relevant chunks
6. 🤖 Gemma 3 generates contextual answers
7. 💬 Chat history is maintained for conversation

---

## 💡 Example Usage

### Input

```id="c3l9ak"
What is the main topic of this document?
```

### Output

```id="q8d2pl"
The document discusses machine learning concepts including supervised and unsupervised learning...
```

---

## 🔑 Key Functions

### 🔹 Create Conversational Chain

```python id="a9s3de"
get_conversational_chain(vector_store)
```

### 🔹 Handle User Input

```python id="z1k8rm"
user_input(user_question)
```

### 🔹 Main App Runner

```python id="p4x7nw"
main()
```

---

## ⚠️ Important Notes

* Make sure Ollama is running locally
* Large PDFs may take time to process
* Ensure PDFs contain extractable text (not scanned images)
* Model runs locally → requires sufficient RAM

---

## 🧩 Future Improvements

* 🖼️ Support for scanned PDFs (OCR)
* 🌐 Web deployment (Streamlit Cloud)
* 🧠 Multiple model support
* 📊 Highlight source text in answers
* 🔐 User authentication

---

## 🤝 Contributing

1. Fork the repository
2. Create a new branch
3. Make changes
4. Submit a Pull Request

---

## 📜 License

This project is licensed under the MIT License.

---

## 👨‍💻 Author

**Shankar Kumar Yadav**
