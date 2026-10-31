# DataInsightBot 🤖📊
### AI-Powered Business Intelligence & Natural Language Data Analytics

[![Live Demo](https://img.shields.io/badge/Live%20Demo-Visit%20Project-brightgreen?style=for-the-badge)](https://data-insight-bot-rif2.vercel.app/)

**DataInsightBot** is an AI-powered business analytics application that enables users to explore and understand business data through natural language questions — without manually writing SQL queries.

Powered by **Google Gemini AI**, the application converts user questions into SQL queries, validates and executes them against a SQLite database, and presents results with AI-generated explanations.

It also includes a Machine Learning module that uses **Random Forest Regression** to predict future sales revenue based on historical sales data.

🔗 **Live Application:** https://data-insight-bot-rif2.vercel.app/

---

## ✨ Key Features

- **Natural Language Analytics:** Ask business questions in everyday language.
- **AI-Powered SQL Generation:** Automatically generates SQL queries using Google Gemini.
- **SQL Query Validation:** Validates generated queries before execution.
- **Database Integration:** Retrieves business insights from a SQLite database.
- **AI-Generated Explanations:** Explains query results in simple, understandable language.
- **Interactive Results:** Displays query outputs in a structured table.
- **Sales Prediction:** Uses a Random Forest Regression model to predict future revenue.
- **Modern Web Interface:** Built with HTML, CSS, and JavaScript.

## 🛠️ Technology Stack

| Category | Technologies |
|---|---|
| Frontend | HTML5, CSS3, JavaScript |
| Backend | Python, FastAPI, Uvicorn |
| Generative AI | Google Gemini API, google-genai |
| Database | SQLite |
| Machine Learning | Scikit-learn, Random Forest Regression |
| Data Processing | Pandas |
| Environment Management | Python dotenv |

## 🏗️ Project Architecture

DataInsightBot follows a workflow that connects natural language processing, SQL generation, database operations, and AI-powered explanations.

```text
       User Question
             |
             v
         Gemini AI
             |
             v
     SQL Query Generation
             |
             v
       SQL Validation
             |
             v
       SQLite Database
             |
             v
        Query Results
             |
             v
       AI Explanation
             |
             v
       Business Insights
```

The Machine Learning module operates separately, using historical sales data to generate revenue predictions through a Random Forest Regression model.

## 📂 Project Structure

```text
DataInsightBot/
│
├── backend/
│   ├── database/
│   ├── chat_service.py
│   ├── database_query.py
│   ├── database_setup.py
│   ├── gemini_service.py
│   ├── insert_data.py
│   ├── main.py
│   ├── ml_prediction.py
│   ├── schema.py
│   ├── sql_validator.py
│   └── test_database.py
│
├── frontend/
│   ├── index.html
│   ├── script.js
│   └── style.css
│
├── .gitignore
└── README.md
```

## ⚙️ Getting Started

Follow these steps to run DataInsightBot locally.

### 1. Clone the Repository

```bash
git clone https://github.com/srivastavaujjwal733-crypto/DataInsightBot.git
cd DataInsightBot
```

### 2. Install Dependencies

```bash
pip install fastapi uvicorn python-dotenv pandas scikit-learn google-genai
```

### 3. Configure Gemini API Key

Create a `.env` file inside the `backend` directory.

```text
backend/.env
```

Add your Gemini API key:

```env
GEMINI_API_KEY=your_api_key_here
```

**Important:** Keep your API key private. Never commit or upload your `.env` file to GitHub.

### 4. Start the Backend Server

Run the following command from the project root directory:

```bash
uvicorn backend.main:app --reload
```

The backend API will be available at:

```text
http://127.0.0.1:8000
```

### 5. Launch the Frontend

Open `frontend/index.html` using the VS Code Live Server extension.

You can now interact with DataInsightBot through the web interface.

## 💡 Example Business Questions

Users can ask questions such as:

- Which department has the highest average salary?
- Which department has the most employees?
- What are the total sales?
- Show me the sales data.
- Which department has the lowest average salary?

DataInsightBot translates these questions into SQL queries, retrieves the relevant information, and explains the results in natural language.

## 📈 Machine Learning – Sales Prediction

DataInsightBot includes a **Random Forest Regression** module for sales revenue prediction.

The module:
- Uses historical sales data.
- Applies a Random Forest Regression algorithm.
- Learns patterns from available data.
- Generates future sales revenue predictions.
- Displays predictions through the web interface.

## 🔐 Security & Validation

- Generated SQL queries are validated before execution.
- The Gemini API key is stored in an environment variable.
- Sensitive environment files are excluded through `.gitignore`.

## 🎓 Key Learning Outcomes

Building DataInsightBot provided practical experience in:

- Natural Language to SQL generation.
- Generative AI and Gemini API integration.
- REST API development using FastAPI.
- SQLite database management and querying.
- SQL query validation.
- Machine Learning with Random Forest Regression.
- Data processing using Pandas.
- Frontend and backend integration.
- API response handling and error management.

## 🚀 Future Improvements

Potential enhancements include:

- Interactive data visualizations and charts.
- Support for additional database systems.
- Advanced business analytics and reporting.
- Improved prediction evaluation and model monitoring.
- User authentication and personalized dashboards.

## 👨‍💻 Author

**Ujjwal Srivastava**

B.Tech – Computer Science & Data Science

[GitHub Profile](https://github.com/srivastavaujjwal733-crypto)

---

⭐ If you find this project interesting, feel free to explore the repository and try the live application.

**Live Demo:** https://data-insight-bot-rif2.vercel.app/
