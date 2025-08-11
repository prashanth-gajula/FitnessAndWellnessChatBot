Fitness & Wellness ChatBot
The Fitness & Wellness ChatBot is an AI-powered conversational assistant designed to guide users in their health and wellness journey. It provides personalized advice on fitness routines, healthy eating, mental well-being, and lifestyle habits.

This project was developed using Flask for the backend and deployed on the AWS Cloud for global accessibility. The chatbot is accessible through a simple web interface, allowing anyone with an internet connection to interact and receive tailored guidance.

Purpose & Benefits
The chatbot aims to make fitness and wellness advice more accessible and interactive for everyone. Instead of reading static articles or following generic workout plans, users can have a two-way conversation with the bot to get information relevant to their needs.

How it helps people:

Beginners can get workout and diet suggestions based on their goals.

Fitness enthusiasts can receive reminders, exercise variations, and nutrition tips.

People with busy lifestyles can ask for quick, effective health hacks.

Anyone can get instant responses instead of waiting for expert consultations.


How It Was Made
Backend: Developed in Flask (Python) to handle chat requests, responses, and session management.

Frontend: HTML templates with CSS and JavaScript for an interactive chat interface.

AI Integration: The chatbot logic connects with AI models to process user input and generate meaningful responses.

Deployment: The project is deployed to AWS Cloud, ensuring scalability and availability for users.


FitnessAndWellnessChatBot/
├── app.py                 # Main Flask application entry point
├── src/                   # Backend logic and helper modules
├── templates/             # HTML templates for the chatbot UI
├── static/                # CSS, JavaScript, and image assets
├── requirements.txt       # Python dependencies
├── Dockerfile             # Containerization setup for deployment
└── .github/workflows/     # CI/CD pipeline configuration

Who Can Use This
Individuals looking to improve fitness and wellness habits.

Personal trainers who want to integrate an AI assistant into their service.

Organizations promoting healthy lifestyles among employees.


Clone & run locally (recommended workflow)

# 1) Clone the repository
git clone https://github.com/prashanth-gajula/FitnessAndWellnessChatBot.git
cd FitnessAndWellnessChatBot

# 2) Create & activate a Conda environment
conda create -n fitness-bot python=3.10 -y
conda activate fitness-bot

# 3) Install dependencies
pip install -r requirements.txt

# 5) Run the app
python app.py
# App should be available at http://localhost:8080

Continuous Integration & Deployment (GitHub Actions)
This repo includes GitHub Actions workflows under .github/workflows/ to build/test the project and deploy changes automatically when you push to the main branch.

What you need to do:

In your GitHub repo, go to Settings → Secrets and variables → Actions and add the necessary secrets (e.g., SECRET_KEY, OPENAI_API_KEY, plus any others your app uses).

Keep the workflow files in .github/workflows/ as-is (or adjust to your environment).

Every time you push changes, Actions will run CI and (if configured) trigger CD to your cloud environment.
