# Django Chat Application

A real-time chat application built using **Django REST Framework**, **Django Signals**, and **ReactJS**.

---

## Features

- **Real-time messaging** between users.
- **User authentication** with profile images.
- Responsive **React.js frontend**.
- Backend powered by **Django REST Framework** and **Django Signals**.

---

## Installation Guide

Follow these steps to set up and run the application on your local machine:

### Backend Setup (Django)

1. **Create a virtual environment**:
   
   ```bash
   virtualenv venv
   ```
   
2. **Activate the virtual environment**:
   
   - For Ubuntu/Linux/MacOS:
     ```bash
     source venv/bin/activate
     ```
     
   - For Windows:
     ```bash
     venv\Scripts\activate
     ```
     
3. Navigate to the `server/` directory:
   
   ```bash
   cd server/
   ```
   
4. **Install dependencies**:
   ```bash
   pip install -r requirements.txt
   ```
5 **Apply database migrations**:
   
   ```bash
   python manage.py migrate
   ```
   
6. **Run the backend server**:
   
   ```bash
   python manage.py runserver
   ```

### Frontend Setup (ReactJS)

1. Navigate to the `client/` directory:
   
   ```bash
   cd client/
   ```

2. **Set the NODE_OPTIONS environment variable**:

   - **For Windows (Command Prompt)**: Use this to set the NODE_OPTIONS environment variable temporarily for the current session:
   
     ```bash
     set NODE_OPTIONS=--openssl-legacy-provider
     npm start
     ```

   - **For Windows (PowerShell)**: In PowerShell, set the environment variable like this:
   
     ```bash
     $env:NODE_OPTIONS="--openssl-legacy-provider"
     npm start
     ```

   - **For macOS/Linux (Terminal)**: Set the environment variable like this:
   
     ```bash
     export NODE_OPTIONS=--openssl-legacy-provider
     npm start
     ```

3. **Install dependencies**:
   
   ```bash
   npm install
   ```

4. **Start the frontend server**:
   
   ```bash
   npm start
   ```
   
---

## How to Use

1. Open your browser and navigate to:
   - Backend: `http://127.0.0.1:8000/`
   - Frontend: `http://localhost:3000/`
2. Open two browser windows or tabs.
3. **Sign up** in both windows using:
   - Name
   - Email
   - Profile image
4. Start chatting between the two browser sessions in real time!

---

## License

This project is licensed under the [MIT License](LICENSE).
