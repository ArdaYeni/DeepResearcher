<img width="1917" height="945" alt="image" src="https://github.com/user-attachments/assets/327fce87-3adf-4f9d-b759-ec9638a13692" />
# Deep Researcher

An AI-powered research assistant that provides **streaming, step-by-step answers** to complex questions.  
Unlike a simple Q&A bot, Deep Researcher is designed to explore topics in depth, structure reasoning clearly, and act like a **thought partner** for literature reviews, brainstorming, and analysis.

---

## ✨ Features
- **Streaming Responses** → Answers are generated word-by-word in real time.  
- **Research Persona** → Encourages detailed, structured, and well-explained outputs.  
- **Interactive Chat** → Users can ask open-ended or technical questions.  
- **Extendable** → Can be adapted into a RAG (Retrieval-Augmented Generation) pipeline by adding PDF/text ingestion.  

---

## 🛠️ Tech Stack
- **[Gradio](https://gradio.app/)** → Interactive web UI  
- **[OpenAI GPT models](https://platform.openai.com/)** → Large Language Model reasoning  
- **[dotenv](https://pypi.org/project/python-dotenv/)** → Manages environment variables  
- (Optional) **SentenceTransformers + FAISS** → For extending into document retrieval  

---

## 📂 Project Structure
```bash
deep-researcher/
│── app.py              # Main Gradio app (streaming chat interface)
│── requirements.txt    # Python dependencies
│── .env.example        # Template for API keys
│── .gitignore          # Ignore secrets, caches, etc.
│── README.md           # Documentation

🔑 Environment Setup

Clone the repository:

git clone https://github.com/<your-username>/deep-researcher.git
cd deep-researcher


Create a virtual environment & install dependencies:

python -m venv venv
source venv/bin/activate   # On Windows: venv\Scripts\activate
pip install -r requirements.txt


Add your API keys in .env:

OPENAI_API_KEY=your_openai_key_here

🚀 Running Locally
python app.py


Gradio will launch at http://localhost:7860
.

Type any research question and receive a streaming, structured answer.
