# Smart-Expense-Tracker-System
A Full Stack Python-based Expense Tracker Application built using Streamlit, FastAPI, and MySQL. This project helps users track daily expenses, analyze spending patterns, and visualize financial data through an interactive dashboard.

*🚀 Key Features : 
   *➕ Add daily expenses with category, amount, and notes
   *📊 View expense breakdown by category
   *📅 Filter expenses using date range
   *📈 Interactive charts for financial insights
   *🗑️ Delete expense records
   *⚡ Fast and lightweight REST API using FastAPI
*💾 Persistent data storage using MySQL
   *🎨 Interactive UI built with Streamlit

🛠️ Tech Stack 
   Frontend (UI): Streamlit (Python-based UI framework)
   Backend (API): FastAPI
   Database: MySQL
   Language: Python

🧩 System Architecture :
       Streamlit UI (Frontend)
              ↓
       FastAPI Backend (REST API)
              ↓
      MySQL Database


 📂 Project Structure:
  backend/   → FastAPI backend (routes, database logic)
  frontend/  → Streamlit user interface
  database/  → SQL schema and data dump


🎯 Project Objective
The main goal of this project is to:

Understand full-stack application development using Python
Learn API creation using FastAPI
Work with relational databases (MySQL)
Build interactive dashboards using Streamlit
Practice real-world project structuring


⚙️ How to Run This Project
1️⃣ Clone the repository
git clone <your-repo-link>
cd Smart-Expense-Tracker

2️⃣ Create virtual environment
python -m venv venv

3️⃣ Activate virtual environment
venv\Scripts\activate   # Windows

4️⃣ Install dependencies
pip install -r requirements.txt

5️⃣ Run Backend (FastAPI)
cd backend
python -m uvicorn server:app --reload

6️⃣ Run Frontend (Streamlit)
cd frontend
python -m streamlit run app.py
