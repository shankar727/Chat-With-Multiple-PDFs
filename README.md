📄🤖 AI PDF Chatbot using Gemma 3 (Ollama + Streamlit)

An intelligent PDF Question-Answering system that allows users to upload documents and ask questions in natural language. Powered by Gemma 3 (Ollama) and LangChain, the app retrieves relevant information and responds conversationally.

🚀 Features

📂 Upload multiple PDF files

🔍 Extract and process text automatically

✂️ Smart text chunking

🧠 Context-aware Q&A using LLM

💬 Conversational memory (chat history)

⚡ Fast local inference with Ollama

🎯 Relevant answer retrieval using vector search

🛠️ Tech Stack

Frontend: Streamlit

LLM: Ollama (Gemma3:4b)

Framework: LangChain

Vector Store: FAISS / Chroma (based on helper)

Language: Python

📂 Project Structure
├── app.py
├── helper.py
├── requirements.txt
└── README.md
⚙️ Installation & Setup
1️⃣ Clone the Repository
git clone https://github.com/your-username/AI-PDF-Chatbot.git
cd AI-PDF-Chatbot
2️⃣ Install Dependencies
pip install -r requirements.txt
3️⃣ Install Ollama

Download from 👉 https://ollama.com/

Then pull the model:

ollama pull gemma3:4b
4️⃣ Run the App
streamlit run app.py

App will open in browser automatically.

🧠 How It Works

📥 User uploads PDF files

📄 Text is extracted using get_pdf_text()

✂️ Text is split into chunks (get_text_chunks())

📦 Vector embeddings are created (get_vector_store())

🔎 Retriever finds relevant chunks

🤖 Gemma 3 generates contextual answers

💬 Chat history is maintained for conversation

💡 Example Usage
Input:
What is the main topic of this document?
Output:
The document discusses machine learning concepts including supervised and unsupervised learning...
🔑 Key Functions
🔹 Create Conversational Chain
get_conversational_chain(vector_store)
🔹 Handle User Input
user_input(user_question)
🔹 Main App Runner
main()
⚠️ Important Notes

Make sure Ollama is running locally

Large PDFs may take time to process

Ensure PDFs contain extractable text (not scanned images)

Model runs locally → requires sufficient RAM

🧩 Future Improvements

🖼️ Support for scanned PDFs (OCR)

🌐 Web deployment (Streamlit Cloud)

🧠 Multiple model support

📊 Highlight source text in answers

🔐 User authentication

🤝 Contributing

Fork the repository

Create a new branch

Make changes

Submit a Pull Request

📜 License

This project is licensed under the MIT License.

👨‍💻 Author

Shankar Kumar Yadav
