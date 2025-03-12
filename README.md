# Task Manager

## Overview
The **Task Manager** is a web-based application built using **Python** and **Flask**, with **MySQL** as the database for storing tasks and user data. The application allows users to create, update, delete, and manage tasks efficiently. It is developed within a Python **virtual environment** for better dependency management and portability.

## Features
- User authentication (Login/Register)
- Create, update, and delete tasks
- Mark tasks as completed/pending
- Categorize tasks by priority or deadlines
- Store task data securely using **MySQL**
- Developed using Flask for backend logic
- Hosted in a Python virtual environment for easy package management

## Technologies Used
- **Backend:** Python, Flask
- **Database:** MySQL
- **Frontend:** HTML, CSS
- **Environment:** Python Virtual Environment

## Installation & Setup
### Prerequisites
Ensure you have the following installed:
- Python (>=3.8)
- MySQL Server
- Flask
- Virtual Environment (venv)

### Step 1: Clone the Repository.

### Step 2: Create a Virtual Environment & Activate It
```bash
python -m venv venv  # Create virtual environment
source venv/bin/activate  # Activate on macOS/Linux
venv\Scripts\activate  # Activate on Windows
```

### Step 3: Install Dependencies
```bash
pip install -r requirements.txt
```

### Step 4: Configure the Database
1. Open MySQL and create a database:
```sql
CREATE DATABASE task_manager;
```
2. Update `config.py` with your MySQL credentials:
```python
DB_NAME = 'task_manager'
DB_USER = 'your_user'
DB_PASSWORD = 'your_password'
DB_HOST = 'localhost'
```

### Step 5: Run Database Migrations
```bash
python migrate.py  # If using Flask-Migrate or similar tools
```

### Step 6: Run the Application
```bash
python app.py
```
The app will run on `http://127.0.0.1:5000/`

## Usage
- Register a new account or log in.
- Create new tasks and manage them in your dashboard.
- Set task priorities, mark them as completed, or delete them.

## Project Structure
```
├── task-manager/
│   ├── venv/ (Virtual Environment)
│   ├── templates/ (HTML Templates)
│   │   ├── base.html
│   │   ├── index.html
│   ├── static/ (CSS, JS, Images)
│   ├── app.py (Main Flask App)
│   ├── config.py (Configuration Settings)
│   ├── models.py (Database Models)
│  
└── README.md
```

## Contribution
Feel free to fork the repository and submit a pull request if you would like to contribute!

## Contact
For any issues or feature requests, please open an issue on the repository.




