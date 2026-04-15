# Smart-Expense-Tracker-System

A Full Stack Python-based Expense Tracker Application built using Streamlit, FastAPI, and MySQL. This project helps users track daily expenses, analyze spending patterns, and visualize financial data through an interactive dashboard.

### 🚀 Key Features
* ➕ **Add daily expenses** with category, amount, and notes
* 📊 **View expense breakdown** by category
* 📅 **Filter expenses** using date range
* 📈 **Interactive charts** for financial insights
* 🗑️ **Delete expense records**
* ⚡ **Fast and lightweight** REST API using FastAPI
* 💾 **Persistent data storage** using MySQL
* 🎨 **Interactive UI** built with Streamlit

### 🛠️ Tech Stack
* **Frontend (UI):** Streamlit (Python-based UI framework)
* **Backend (API):** FastAPI
* **Database:** MySQL
* **Language:** Python

### 🧩 System Architecture
Streamlit UI (Frontend)  
       ↓  
FastAPI Backend (REST API)  
       ↓  
MySQL Database

### 📂 Project Structure
* `backend/` → FastAPI backend (routes, database logic)
* `frontend/` → Streamlit user interface
* `database/` → SQL schema and data dump

### 🎯 Project Objective
The main goal of this project is to:
1. Understand full-stack application development using Python
2. Learn API creation using FastAPI
3. Work with relational databases (MySQL)
4. Build interactive dashboards using Streamlit
5. Practice real-world project structuring

### ⚙️ How to Run This Project

**1️⃣ Clone the repository**
```bash
git clone [https://github.com/krishnegowda9/Smart-Expense-Tracker-System.git](https://github.com/krishnegowda9/Smart-Expense-Tracker-System.git)
cd Smart-Expense-Tracker-System

2️⃣ Create virtual environment

Bash
python -m venv venv
3️⃣ Activate virtual environment

Bash
# Windows
venv\Scripts\activate
# Mac/Linux
source venv/bin/activate
4️⃣ Install dependencies

Bash
pip install -r requirements.txt
5️⃣ Run Backend (FastAPI)

Bash
cd backend
python -m uvicorn server:app --reload
6️⃣ Run Frontend (Streamlit)

Bash
cd frontend
python -m streamlit run app.py

