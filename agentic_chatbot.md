# 🤖 Personalized Agentic AI Chatbot with Tool Use

## 🧪 Title: Building a Personalized Agentic AI Chatbot Using Gradio, LLM APIs, and Tool Integration

As part of my self-guided exploration into Agentic AI systems, I developed an interactive chatbot using Gradio, Python, and large language model APIs. The goal was to build a personalized assistant that could answer questions about my background and projects by referencing a structured profile stored in a PDF and a summary text file. The agent could also trigger tools for specific user intents such as irrelevant queries or contact requests.

## 🎯 Motivation

Agentic AI systems are characterized by their ability to reason, access external tools, and adapt behavior based on user goals. This project was designed to help me understand how to ground LLMs in local knowledge and enable minimal autonomy through tool use.

## 🏗️ Architecture

- **Frontend**: Built using Gradio, providing a web-based user interface.  
- **Language Model**: Integrated either OpenAI GPT or Groq LLaMA2 via their respective APIs.  
- **Knowledge Base**: Extracted and preprocessed text from a PDF and summary text file  
- **Retrieval & Prompting**:
  - Embedded files for similarity-based retrieval  
  - Custom system prompt instructing the LLM to restrict answers to file-based knowledge and tool schema  
- **Tool Integration**: Python-based tools triggered by specific intents:
  - Irrelevant queries → push notifications  
  - Contact intent (e.g., user provides email) → push notifications

## 📈 Outcomes

The chatbot demonstrated context awareness, memory over personalized content, and basic decision-making via tool calls.

The chatbot handled relevant profile queries like:  
- “What is your educational background?”  
- “Have you worked on AI-related projects?”  

Tool use was triggered for:  
- Irrelevant queries (e.g., “What’s the weather in Dubai?”)  
- User contact attempts (e.g., “Can I reach out? My email is…”)

## 📚 Learnings

- Grounding LLMs in personal data significantly improves answer relevance  
- System prompts with structured tool schemas guide model behavior effectively.  
- Tool use adds a layer of autonomy, allowing fallback actions for out of scope queries.  
- Gradio’s UI enabled fast testing with end users.
