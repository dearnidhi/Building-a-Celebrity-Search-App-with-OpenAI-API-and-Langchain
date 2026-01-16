Celebrity Search with LangChain & OpenAI API is a Streamlit-based web app that lets users input a celebrity’s name and automatically:
Retrieves information about the celebrity.
Finds their date of birth.
Lists major world events around that date.
It uses LangChain to create a multi-step chain of prompts with OpenAI’s LLM, and ConversationBufferMemory to track context for better responses.

# 🌟 Celebrity Search with LangChain & OpenAI API

## 📌 Overview

This web application allows users to search for celebrities and receive:

- Basic information about the celebrity
- Their date of birth
- Significant global events around their birthdate

The app is built with **Streamlit** and uses **LangChain** to structure sequential prompts to OpenAI’s language model. Conversation memory ensures coherent multi-step interactions.

---

## 🛠️ Tech Stack

- Python  
- Streamlit  
- LangChain  
- OpenAI API  

---

## ▶️ Installation & Setup

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/your-username/celebrity-search-langchain.git
cd celebrity-search-langchain

2️⃣ Create & Activate Virtual Environment
python -m venv venv
source venv/bin/activate     # Windows: venv\Scripts\activate

3️⃣ Install Dependencies
pip install -r requirements.txt

4️⃣ Configure OpenAI API Key
Create a constant.py file in the root directory:
openai_key = "your_openai_api_key_here"

▶️ Run the Application
streamlit run app.py
The application will be accessible at:
http://localhost:8501

🧠 How It Works

User inputs a celebrity name.
Step 1: LangChain fetches general info about the celebrity.
Step 2: LangChain queries for the celebrity’s date of birth.
Step 3: LangChain lists 5 major world events around that date.
Results are displayed on the web app with expandable sections for context.

⚠️ Notes

Requires a valid OpenAI API key
Responses depend on the OpenAI model used
Intended for demo and educational purposes
