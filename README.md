Markdown
# AI-Medical-Chatbot 🩺
**A Production-Ready Healthcare Assistant using RAG (Retrieval-Augmented Generation)**

This project is a sophisticated medical inquiry system developed as a Capstone Project for MS in Data Science. It utilizes a Retrieval-Augmented Generation (RAG) architecture to provide accurate, context-aware answers from a validated medical encyclopedia.

## 🚀 Features
- **Intelligent Retrieval:** Uses Pinecone Vector DB to search through thousands of medical data chunks.
- **LLM Integration:** Powered by Google Gemini 1.5 Flash for high-speed, cost-effective reasoning.
- **Modern RAG Pipeline:** Built with LangChain for seamless orchestration between embeddings and the LLM.
- **Web Interface:** A clean, responsive Flask-based UI for real-time user interaction.
- **Cloud Native:** Architecture ready for AWS deployment via Docker and GitHub Actions.

## 🛠️ Tech Stack
- **Language:** Python 3.10
- **Orchestration:** LangChain
- **LLM:** Google Gemini 1.5 Flash
- **Embeddings:** HuggingFace `all-MiniLM-L6-v2`
- **Vector Store:** Pinecone
- **Frontend:** Flask (HTML/CSS/JS)

---

## 🏃 How to Run

### 1. Clone the Repository
```bash
git clone [https://github.com/Bhawana-Zende/AI-Medical-Chatbot.git](https://github.com/Bhawana-Zende/AI-Medical-Chatbot.git)
cd AI-Medical-Chatbot
2. Setup Environment
Ensure you have Conda installed.

Bash
conda create -n medibot python=3.10 -y
conda activate medibot
pip install -r requirements.txt
3. Configure Credentials
Create a .env file in the root directory and add your API keys:

Ini, TOML
PINECONE_API_KEY = "your_pinecone_key"
GOOGLE_API_KEY = "your_google_gemini_key"
4. Run the Application
Bash
# Optional: Only run if you need to re-index the medical PDF
# python store_index.py

# Launch the Flask Server
python app.py
Open your browser and navigate to http://127.0.0.1:8080.

☁️ AWS CI/CD Deployment
The repository includes a GitHub Actions workflow to automate deployment:

Build: Dockerizes the Flask application.

Push: Sends the image to Amazon ECR.

Deploy: Pulls and runs the container on an Amazon EC2 instance.

Required GitHub Secrets:
AWS_ACCESS_KEY_ID

AWS_SECRET_ACCESS_KEY

AWS_DEFAULT_REGION

ECR_REPO

PINECONE_API_KEY

GOOGLE_API_KEY

Developed by Bhawana Zende 


### To update your GitHub now:
1.  **Save** this into your `README.md` file in VS Code.
2.  **Run** these commands in your terminal:
    ```zsh
    git add README.md
    git commit -m "Finalized professional README documentation"
    git push origin main
    ```
