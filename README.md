# 💰 Smart Expense Tracker System

A full-stack financial tracking application featuring a **FastAPI** backend for data management and an interactive **Streamlit** dashboard for seamless expense analytics.

---

## 📌 Project Overview

This repository provides a complete end-to-end solution for managing daily expenses, viewing visual analytics, and storing transactional logs safely.

* **Frontend**: Built with Streamlit for clean visual reporting and data input.
* **Backend**: Powered by FastAPI for high-performance API endpoints and data persistence.

---
```mermaid
graph TD
    classDef ui fill:#1f2937,stroke:#3b82f6,stroke-width:2px,color:#fff;
    classDef api fill:#111827,stroke:#10b981,stroke-width:2px,color:#fff;
    classDef db fill:#0f172a,stroke:#8b5cf6,stroke-width:2px,color:#fff;
    classDef log fill:#334155,stroke:#f59e0b,stroke-width:2px,color:#fff;

    subgraph Frontend ["🎨 Frontend Tier (Streamlit UI - app.py)"]
        A["Add / Update UI<br/><i>(add_update_ui.py)</i>"]:::ui
        B["Analytics & Insights UI<br/><i>(analytics_ui.py)</i>"]:::ui
    end

    subgraph Backend ["⚡ Backend API Tier (FastAPI - server.py)"]
        C["API Routes & Request Handlers<br/><i>(GET/POST/PUT/DELETE)</i>"]:::api
        D["Logging Engine<br/><i>(logging_setup.py)</i>"]:::log
    end

    subgraph Storage ["💾 Persistence Tier"]
        E["Database Helper Utilities<br/><i>(db_helper.py)</i>"]:::db
        F["Database Storage<br/><i>(MySQL / SQLite Schemas)</i>"]:::db
    end

    A -->|"HTTP POST / PUT (Expense Records)"| C
    B -->|"HTTP GET (Fetch Aggregated Analytics)"| C
    C -->|"Log Requests & Operational Events"| D
    C -->|"Executes Query Operations"| E
    E -->|"Reads / Writes Data"| F
```
    
## 📁 Repository Structure

```text
Smart-Expense-Tracker-System/
│
├── 📂 database/          # Database files and schemas
├── 📄 app.py             # Streamlit main entry point
├── 📄 add_update_ui.py   # UI module for adding & modifying records
├── 📄 analytics_ui.py    # UI module for visual insights & charts
├── 📄 db_helper.py       # Database utility & connection functions
├── 📄 server.py          # FastAPI server entry point
├── 📄 logging_setup.py   # Logging configuration
├── 📄 requirements.txt   # Python dependencies
└── 📄 README.md          # Project documentation

1. Clone the Repository
git clone [https://github.com/krishnegowda9/Smart-Expense-Tracker-System.git](https://github.com/krishnegowda9/Smart-Expense-Tracker-System.git)
cd Smart-Expense-Tracker-System

2. Install Dependencies
Ensure you have Python 3.8+ installed, then run:
pip install -r requirements.txt

3. Launch the FastAPI Backend
Start the backend server on http://localhost:8000:
uvicorn server:app --reload

4. Launch the Streamlit Frontend
In a new terminal window, run the UI:
streamlit run app.py

🛠️ Tech Stack
Language: Python

Backend: FastAPI, Uvicorn

Frontend: Streamlit

Database: MySQL / SQLite (configured via db_helper.py)
