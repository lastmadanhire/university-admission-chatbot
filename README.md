
# University Enrollment and admissions ChatBot

The university admission chatbot is a useful tool designed to provide assistance and information by answering general student queries during university admissions using state-of-the-art language models and vector stores.

### Problem Identified:
Handling a high volume of inquiries during university admissions can overwhelm staff and significantly slow down response times. Many students seek general information, which can lead to delays as staff address repetitive queries manually. This inefficiency not only strains resources but also negatively impacts the user experience. To address these challenges, we are developing a university admission chatbot that leverages Generative AI and advanced language models to provide instant, accurate responses, streamline the admissions journey and reduce the workload on university staff.

### Project objectives:

- To develop a university chatbot to assist with student queries on admissions processes and enquiries using large language models and vector stores.

- To create a Flask FastAPI-based API with robust endpoints for user authentication, chatbot interaction and admin operations including data embedding and CRUD functions.

- To create a document embedding system allowing admins to mange data files in the vector database ensuring up-to-date and correct data.



### Product Impact:
Transformed the university admissions process by efficiently handling high inquiry volumes, streamlining the journey with instant responses, reducing staff workload and enhancing the institution's reputation for technological innovation.

## Prerequisites

Before you can start using the ChatBot, make sure you have the following prerequisites installed on your system:

- Python 3.9 or higher but I recommend python 3.12
- Required Python packages (all packages are in requirement.txt)

### Required libraries:
-flask
-flask_cors
-google-generativeai
-python-dotenv
-langchain
-pypdf
-chromadb
-faiss-cpu
-fastapi
-pydantic
-uvicorn
-requests
-starlette
-mysql-connector-python
-fastapi_jwt_auth
-passlib

## Installation

1. Clone this repository to your local machine.

2. Create a Python virtual environment (optional but recommended):

    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows, use: venv\Scripts\activate.bat
    ```

3. Install the required Python packages:

    ```bash
    pip install -r requirements.txt
    ```

4. Create .env file for creating environment variables.
5. Add your Googl API key variable in the file. You can get your API key from here
- For Google API Key: https://makersuite.google.com/app/apikey

    ```bash
    GOOGLE_API_KEY="Insert your google API key here"
    ```
## Creating and importing database on MySQL

1. Open xamp or MySQL workbench to start the db server. 
    import database located inside backend data folder
    makesure the database the db server run on port 3306

## Run backend API on local server

1. Open cmd in the root folder and write this command to run the live server. 
    ```bash
    cd backend
    uvicorn main:app --reload
    the backend API server will be up on port 8000 

## Run frontend server

1. Open cmd in the root folder and write this command to run the live server. 
    ```bash
    cd frontend
    python app.py
    the frontend server will be up on port 5000 
    ```
   
## API endpoints

- / -> For accessing homepage
- /login -> For accessing login
- /admin -> For accessing Knowledgebase (its protected endpoint)
- /users -> For accessing registered users (its protected endpoint)

## My contact in case
Refere to my profile

