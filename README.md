# AI-Study-Guide-Langgraph
# 🤖 AI Study Guide – LangGraph

An AI-powered personalized learning assistant built using **Streamlit, LangGraph, LangChain, and Groq API**. It helps students learn different technical subjects through interactive conversations, structured explanations, and practical examples.

## 🚀 Features

- **Multiple Learning Modules:** Python, SQL, Power BI, EDA, Machine Learning, Deep Learning, Generative AI, and Agentic AI.
- **AI-Powered Learning:** Generates clear and structured answers using an LLM.
- **LangGraph Workflow:** Uses a graph-based workflow to validate questions and generate relevant answers.
- **Question Validation:** Checks whether questions are related to the selected learning module.
- **Interactive Chat:** Maintains conversation history for contextual responses.
- **Workflow Visualization:** Displays the LangGraph workflow diagram.
- **Download Conversation:** Allows users to download their chat history.
- **User Feedback:** Collects feedback through star ratings.

## 🛠️ Technologies Used

- Python
- Streamlit
- LangGraph
- LangChain
- Groq API
- OpenAI GPT-OSS 20B model (via Groq)
- python-dotenv

## 📂 Project Structure

```text
AI-Study-Guide/
│
├── app.py
├── requirements.txt
├── README.md
├── .env
└── .gitignore
```

## ⚙️ Installation and Setup

### 1. Clone the Repository

```bash
git clone YOUR_GITHUB_REPOSITORY_URL
```

### 2. Navigate to the Project Folder

```bash
cd AI-Study-Guide
```

### 3. Create a Virtual Environment

```bash
python -m venv venv
```

### 4. Activate Virtual Environment

**Windows:**

```bash
venv\Scripts\activate
```

### 5. Install Dependencies

```bash
pip install -r requirements.txt
```

### 6. Configure Groq API Key

Create a `.env` file in the root project directory.

Add your API key:

```env
gem=YOUR_GROQ_API_KEY
```

Replace YOUR_GROQ_API_KEY  with your actual API key.

### 7. Run the Application

```bash
streamlit run app.py
```

The application will open in your browser.

## 🔄 LangGraph Workflow

The application uses LangGraph to manage the AI learning workflow.

```text
       START
         |
         v
  Validate Module
         |
         v
   Check Question
      /       \
     /         \
   YES          NO
    |            |
    v            v
Generate       Invalid
 Answer        Response
    |            |
    v            v
    END          END
```

### Workflow Explanation

1. **Validate Module:** Checks whether the user's question is relevant to the selected learning module.
2. **Conditional Routing:** Routes the question based on the validation result.
3. **Generate Answer:** Generates a contextual response using the Groq LLM.
4. **Invalid Response:** Displays a message when the question is unrelated to the selected module.
5. **END:** Completes the workflow.

## 📚 Available Learning Modules

1. Python
2. SQL
3. Power BI
4. Exploratory Data Analysis (EDA)
5. Machine Learning
6. Deep Learning
7. Generative AI
8. Agentic AI

## 🔐 API Configuration

This project uses the Groq API with the `openai/gpt-oss-20b` model through LangChain's ChatGroq integration.

The API key is loaded securely using `python-dotenv` or Streamlit secrets.

## 🎯 Project Objective

The main objective of this project is to provide students with a personalized AI learning assistant that supports technical learning, improves conceptual understanding, and encourages interactive learning through Generative AI and Agentic AI concepts.

## 👩‍💻 Author

**Nethravathi S**

GitHub: [https://github.com/Nethravathi-S](https://github.com/Nethravathi-S)

---

⭐ If you find this project useful, consider giving it a star!
