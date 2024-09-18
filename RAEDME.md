# Flask and MongoDB Project

This project consists of two main components: a Flask web application and a MongoDB interaction script. It demonstrates basic web development with Flask and database operations with MongoDB.

## Components

1. `app.py`: Flask Web Application
2. `mongo-practice.py`: MongoDB Interaction Script

## 1. Flask Web Application (`app.py`)

### Features:
- Serves static files from a custom folder
- Implements session management
- Handles various routes including:
  - Home page with language detection
  - Hello page with name parameter
  - Talk page using session data
  - Form submission handling
  - Sum calculation based on user input
  - User-specific greetings with dynamic routing

### Routes:
- `/`: Home page
- `/hello`: Greets user and stores name in session
- `/talk`: Uses session data to greet user
- `/page`: Renders a template
- `/submited`: Handles form submission (POST)
- `/getSum`: Calculates sum based on user input (POST)
- `/test`: Redirects to Google
- `/user/<username>`: Dynamic routing for user greetings

### Setup:
1. Install Flask: `pip install flask`
2. Run the application: `python app.py`
3. Access the web application at `http://localhost:3000`

## 2. MongoDB Interaction Script (`mongo-practice.py`)

### Features:
- Connects to MongoDB Atlas
- Performs various database operations:
  - Sorting and filtering data
  - Updating documents
  - Deleting documents
  - Inserting single and multiple documents

### Setup:
1. Install required packages: `pip install pymongo python-dotenv`
2. Create a `.env` file with your MongoDB Atlas credentials:
   ```
   USER=your_username
   PASSWORD=your_password
   ```
3. Run the script: `python mongo-practice.py`

### Note:
Most database operations in this script are commented out. Uncomment the relevant sections to perform specific operations.

## Requirements
- Python 3.x
- Flask
- pymongo
- python-dotenv

## Getting Started
1. Clone this repository
2. Install the required packages: `pip install flask pymongo python-dotenv`
3. Set up your MongoDB Atlas account and update the connection string in `mongo-practice.py`
4. Create a `.env` file with your MongoDB credentials
5. Run `app.py` for the web application
6. Run `mongo-practice.py` to interact with MongoDB (modify as needed)

## Security Note
Ensure that your `.env` file is included in your `.gitignore` to keep your credentials secure.
