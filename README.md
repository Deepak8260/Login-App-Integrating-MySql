# Flask Login Page with MySQL Integration

Welcome to the **Flask Login Page with MySQL Integration**! This project demonstrates how to build a simple login and signup system using Flask and MySQL. Below is a detailed guide to help you set up and run the project on your local machine. **Please note:** Comments have been added to indicate where screenshots (SS) should be included for additional clarity.

---

## Features
- User-friendly login and signup pages with form validation.
- Integration with MySQL for user data storage.
- Modular and secure structure using environment variables.
- Attractive and responsive design with Glassmorphism effects.

---

## Tools and Technologies Used
This project is built using the following tools and technologies:
- **Python**: Core programming language.
- **Flask**: Lightweight web framework for building the application.
- **MySQL**: Relational database for user data storage.
- **MySQL Connector**: Python library to connect Flask with MySQL.
- **HTML/CSS**: For building the front-end interface.
- **dotenv**: To securely manage environment variables.
- **VS Code**: Recommended IDE for writing and debugging the code.

---

## Prerequisites
Before running the project, ensure you have the following installed:
1. **Python 3.7+**
2. **MySQL Server**
3. **pip** (Python package manager)

---

## Folder Structure
```
LOGIN PAGE WITH MYSQL
|
|-- mysql/             # Virtual environment (excluded in .gitignore)
|-- static/            # Static files (CSS, JS, images)
|   |-- style.css      # Styling for the pages
|-- templates/         # HTML templates
|   |-- login.html     # Login page
|   |-- signup.html    # Signup page
|   |-- response.html  # Response page
|-- .env               # Environment variables (excluded in .gitignore)
|-- .gitignore         # Files to exclude from Git
|-- app.py             # Flask application entry point
|-- database.py        # Database connection and utility functions
|-- requirements.txt   # Python dependencies
```

---

## Setup Guide

### Step 1: Clone the Repository
1. Clone this repository to your local machine:
   ```bash
   git clone https://github.com/your-username/your-repository-name.git
   ```
   ![alt text](/Screenshots/1.png).

2. Navigate/Switch to the respective directory
   ```bash
    cd your-repository-name
   ```
   ![alt text](/Screenshots/2.png).
   
---

### Step 2: Create a Virtual Environment
1. Open the terminal in VS Code by clicking on the **Terminal** option in the top menu and selecting **New Terminal**.
   ![alt text](/Screenshots/terminal.png).
2. Run the following command to create a virtual environment:
   ```bash
   python -m venv mysql
   ```
   ![alt text](/Screenshots/3.png).

---

### Step 3: Activate the Virtual Environment
1. Activate the virtual environment using the following command:
   ```bash
    mysql/bin/activate   # On Windows: mysql\Scriptsctivate
   ```
   ![alt text](/Screenshots/4.png).
   
---

### Step 4: Install Dependencies
1. Install all required Python packages:
   ```bash
   pip install -r requirements.txt
   ```
   ![alt text](/Screenshots/5.png).

---

### Step 5: Configure the `.env` File
1. Create a `.env` file in the root directory with your database credentials:
   ```env
   DB_HOST=localhost
   DB_USER=your_user_name
   DB_PASSWORD=your_password
   DB_NAME=db_name
   ```
   ![alt text](/Screenshots/6.png).

   
---

### Step 6: Set Up the Database
1. Log in to your MySQL server or create a new connection in mysql workbench and create the database:
   ```sql
   CREATE DATABASE db_name;
   ```
   ![alt text](/Screenshots/7.png).

---

### Step 7: Run the Flask Application
1. Start the Flask server:
   ```bash
   python app.py
   ```
   ![alt text](/Screenshots/8.png).

---

### Step 8: Application Walkthrough
#### Login Page
1. Open the login page at `http://127.0.0.1:5000/login`.
   ![alt text](/Screenshots/9.png).
   
3. Enter valid credentials and click **Login**.
   - If the credentials are correct:
     ![alt text](/Screenshots/login.png).
   - Validate in the mysql workbench
     ![alt text](/Screenshots/new.png).
   - If the credentials are incorrect:
     ![alt text](/Screenshots/11.png).

#### Signup Page
1. If you are not registered, click the **Sign up here** link at the bottom of the login page.
   ![alt text](/Screenshots/12.png).
2. Fill in the required details and click **Sign Up**.
   ![alt text](/Screenshots/13.png).
3. After successful signup, you will see a confirmation message.
   ![alt text](/Screenshots/14.png).
4. Return to the login page and log in with the newly registered credentials.
   ![alt text](/Screenshots/15.png).
   ![alt text](/Screenshots/login.png).
---

## Best Practices
1. **Environment Variables**: Use the `.env` file to securely store sensitive information like database credentials. Never commit this file to version control.
2. **Virtual Environment**: Always use a virtual environment to isolate project dependencies.
3. **Error Handling**: Implement proper error handling for database connections and user inputs.
4. **Database Security**: Hash user passwords before storing them in the database for enhanced security.
5. **Code Modularity**: Keep database logic and application logic separate for maintainability.

---

## Dependencies
All dependencies are listed in `requirements.txt` and include:
- `flask`
- `mysql-connector-python`
- `python-dotenv`

Install them using:
```bash
pip install -r requirements.txt
```

---

## .gitignore
Sensitive and unnecessary files are excluded using the `.gitignore` file:
```
# Virtual environment
mysql/

# Environment variables
.env

# Bytecode files
__pycache__/
*.pyc

# Jupyter Notebook checkpoints
.ipynb_checkpoints/
```

---

## Contributing
Feel free to fork this repository and make your own improvements. If you'd like to contribute, submit a pull request with a detailed description of the changes.

---

## License
This project is open-source and available under the [MIT License](LICENSE).

---

## Support
If you encounter any issues or have questions, feel free to open an issue in the repository or contact me through any of the following channels:

- 📧 [E-Mail](mailto:kd.codegeek@gmail.com)
- 💼 [LinkedIn](https://www.linkedin.com/in/deepak-kumar-mohanty-09aa59230/)
- 🐦 [Twitter](https://x.com/KumarDeepak2k4)

---

Thank you for using the Flask Login Page with MySQL Integration! 🎉
