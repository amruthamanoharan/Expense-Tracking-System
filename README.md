# Expense Tracking System 

## **Overview**
The Expense Tracking System is an end-to-end Python project designed to manage and analyze personal or organizational expenses. Built with a combination of **FastAPI**, **Streamlit**, and **MySQL**, this project demonstrates the integration of backend development, database interactions, and frontend user interface design. 


## **Project Features**
### 1. **Backend (FastAPI)**
- Developed RESTful APIs using FastAPI to handle expense-related operations.
- Key features include:
  - Adding, updating, and deleting expenses.
  - Fetching expenses by date.
  - Generating analytical summaries based on date ranges or categories.
- Tested APIs using **Postman**.

### 2. **Frontend (Streamlit)**
- Designed a user-friendly interface with Streamlit.
- Tabs for:
  - Adding/updating expenses.
  - Viewing analytics by category for a selected date range.
  - Viewing analytics by month.
- Dynamic visualizations using bar charts and tables to display insights.

### 3. **Database (MySQL)**
- MySQL database used to store and manage expense data.
- Tables for:
  - Expense records (amount, category, date, notes).

### 4. **Testing**
- Unit tests written for backend functions to ensure robust and reliable operations.
- Used **Pytest** for testing database helper functions and API endpoints.


## **Skills Demonstrated**
- **Backend Development**: FastAPI, Pydantic models, API design, database integration.
- **Frontend Development**: Streamlit, interactive data visualization.
- **Database Management**: MySQL schema design, CRUD operations.
- **Testing**: Pytest, unit testing, and Postman API testing.
- **Additional Skills**: Context managers, logging, modular design.


## **Folder Structure**
```
expense-tracking-system/
├── backend/
│   ├── db_helper.py             # Database helper functions
│   ├── logging_setup.py         # Logger configuration
│   ├── server.py                # FastAPI backend implementation
├── database/
│   ├── expense_db_creation.sql  # MySQL database schema
├── frontend/
│   ├── add_update.py            # Backend integration for expense management
│   ├── add_update_ui.py         # Backend integration for expense management    |
│   ├── analytics_by_category.py # Category-wise expense analytics
│   ├── analytics_by_months.py   # Month-wise expense analytics
│   ├── analytics_ui.py          # analytics ui
│   ├── app.py                   # Streamlit app main entry point
├── tests/
│   ├── backend/
│   │   ├── test_db_helper.py    # Unit tests for backend database helper functions
│   ├── frontend/                
│   │   ├── conftest.py          # Frontend-specific Pytest configuration 
│   ├── conftest.py              # Pytest configuration
├── README.md                    # Project documentation
├── requirements.txt             # Lists the required Python packages.
```

## **Key Functionalities**
### **1. Add/Update Expenses**
- Enter expenses by selecting a date, amount, category (e.g., Rent, Food, Shopping), and adding notes.

### **2. Analytics by Category**
- View a breakdown of expenses by category over a specified date range.
- Includes bar charts and tables for visual insights.

### **3. Analytics by Month**
- Summarizes monthly expenses, showing trends across different months.
- Displays visualizations and tables for better understanding.



## **Setup Instructions**
### Prerequisites
- Python 3.8 or higher
- MySQL database
- Libraries: FastAPI, Streamlit, mysql-connector-python, pytest, requests

### Steps
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/expense-tracking-system.git
   cd expense-tracking-system ```
### **Set up the database**
- Run the script in `database/expense_db_creation.sql` to create the required schema.

### **Install dependencies**
```bash
pip install -r requirements.txt
```

### **Start the FastAPI backend**
```bash
uvicorn backend.server:app --reload
```

### **Run the Streamlit frontend**
```bash
streamlit run frontend/app.py
```

### **Access the application**
- FastAPI API docs: http://localhost:8000/docs
- Streamlit app: http://localhost:8501


## Key Learnings
- Building end-to-end applications with Python.
- Integration of backend APIs with frontend interfaces.
- Managing relational databases for real-world applications.
- Developing and testing robust, modular codebases.










