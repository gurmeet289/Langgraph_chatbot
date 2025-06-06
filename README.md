# Langgraph_chatbot

# 💬 LangGraph Chatbot with Groq and Real-Time Search

An intelligent, dynamic chatbot built using **LangGraph**, **Groq's LLM (Gemma2-9b-It)**, and **Streamlit**, with the ability to invoke **real-time search tools** like Tavily when the model needs external help answering your questions.

---

## 🚀 Demo

Ask any question — the chatbot will either respond directly via LLM or invoke a real-time web search if needed using Tavily.

![image1](https://github.com/user-attachments/assets/d24b025e-1713-4f10-9bc3-a46555e0ba9d)  <!-- (optional: add a screenshot of your Streamlit UI here) -->

---

## 📂 Project Structure

langgraph-chatbot/
│

├── chatbot_with_langgraph/

│   ├── app.py         # Streamlit frontend app

│   └── bot.py         # LangGraph logic and tool orchestration

│

├── .env               # Your API key should go here (not committed)

├── requirements.txt   # All required packages

└── README.md          # This file

---

## 🔧 Features

    💡 Uses LangGraph to create dynamic conversational workflows (LLM → Tool → LLM).
    
    ⚡ Powered by Groq's LLM (Gemma2-9b-It) for ultra-fast response times.
    
    🌐 Integrates Tavily Search Tool to fetch real-time web answers.
    
    🖥️ Simple Streamlit UI for interactive usage.
    
    🔁 Automatically routes between LLM and tools based on context.
    
    🔐 Securely loads API keys from .env.

## How It Works -

    1) User submits a question via the Streamlit frontend.
    
    2) LangGraph routes the message to the Groq LLM.
    
    3) If the LLM detects it needs a tool (like Tavily), it routes accordingly.
    
    4) Final answer is displayed to the user.

## 📦 Installation -

    1. Clone the repo

        git clone https://github.com/gurmeet289/langgraph-chatbot.git
        cd langgraph_chatbot

    2. Create & activate virtual environment

        ### For Windows:
            
            python -m venv venv_lang_chatbot
            venv_lang_chatbot\Scripts\activate
        
        #### For Unix/Mac:
            
            python3 -m venv venv_lang_chatbot
            source venv_lang_chatbot/bin/activate

    3. Install dependencies

        pip install -r requirements.txt

## 🔑 API Key Setup

    1. Create a .env file in the root directory:

        GROQ_API_KEY=your_groq_api_key_here

    2. Get your Groq API Key:

        - Visit Groq Console

        - Generate a key and paste it in .env

## 🏁 Run the App

    streamlit run app.py
