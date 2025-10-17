# AIFL Capstone Project Guide- Readme

Project Name: AI-Powered French Learning (AIFL)

## Group Members 
- Kusha Sharma


## Description:
The AI-Powered French Learning (AIFL) project is a web-based application developed to assist students studying French as a second language at Arizona State University (ASU). It uses large language models (LLMs) and generative AI (GenAI) to personalize language practice, focusing on vocabulary memorization and verb conjugation drills. The goal is to provide an engaging supplementary learning tool that complements in-class and homework activities, supporting students' progress through personalized AI-driven feedback and progress tracking

## Table of Contents
- [Target Users](#tu)
- [Features](#f)
- [User Experience Evaluation](#uee)
- [Technologies Used](#techu)
- [Setup Instructions](#si)


<a name="tu"></a>
### Target Users
This tool is designed for ASU students enrolled in online, hybrid, or in-person French courses who need supplemental practice with vocabulary and verb conjugations outside of class. It is also ideal for learners seeking personalized feedback on their progress through AI-driven interaction. The AI chatbot serves as a personalized tutor, prompting students to select specific areas of French learning they would like to practice. Once a topic is chosen, the chatbot provides immediate, tailored feedback on their responses, helping reinforce correct usage and improve language skills. To track progress, the application records total time spent and questions answered, displaying these insights on a dashboard for students to monitor their learning journey.



<a name="f"></a>
### Features

- User Authentication: Students must log in to access the tool.
- Data Persistence: User interactions and progress must be stored in and retrieved from the database.
- Generative AI Integration: The tool connects to a generative AI API (e.g., OpenAI GPT) on the backend.
- Progress Identification: Weekly learning activities are tracked and stored.

<a name="uee"></a>
### User Experience Evaluation
- Usability Testing: Tested with multiple users to evaluate the usability of the tool, collect feedback, and assess its effectiveness. This involved student trials, surveys, or direct observations.
- Metrics to Focus On: Usability, ease of learning, and satisfaction with AI feedback.

<a name="techu"></a>
### Technologies Used

- Backend (Flask): Python framework to handle API interactions and connect with the OpenAI API for generating responses.
- Frontend (Angular): Used to create a user-friendly interface.
- Database (SQLite): For storing and retrieving user data, progress, and interactions.
- Generative AI: OpenAI API to generate questions and responses for french learning. The chatbot uses GPT-4 to interact with the user. 

<a name="si"></a>
## Setup Instructions

### For Backend (Flask):

#### 1. Create a Virtual Environment
Navigate to the project directory and create a virtual environment:
```
cd Flask_Rest_API
```
•	On macOS and Linux:
```
python3 -m venv env
```
•	On Windows:
```
python -m venv env
```
This will create a new directory called env in your project folder to store the virtual environment.

#### 2. Activate the Virtual Environment
   
•	On macOS and Linux:
```
source env/bin/activate
```
•	On Windows:
```
.\env\Scripts\activate
```
Once activated, your command prompt should show (env) at the beginning.

#### 3. Install Dependencies
```
pip install -r requirements.txt
```

#### 4. Run backend
After setting up the environment and installing dependencies, you can run your application:
```
python3 run.py
```

#### *** To Install and Save Dependencies (Optional)
With the virtual environment activated, install the required packages:

•	On macOS and Linux:
```
pip3 install flask flask_sqlalchemy flask_restful flask_cors
```
•	On Windows:
```
pip install flask flask_sqlalchemy flask_restful flask_cors
```
To save the dependencies to a requirements.txt file for easy setup later, run:
```
pip freeze > requirements.txt
```
In the future, others (or you, if you set up a new environment) can install all dependencies from this file using:
```
pip install -r requirements.txt
```
### For Frontend (Angular):

#### 1. Navigate to the project directory:
```
cd Angular_Client
```
#### 2. Run frontend
```
ng serve
```

