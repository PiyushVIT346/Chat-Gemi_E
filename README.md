
Here’s a sample content for the README.md file that explains how your Flask application works, its purpose, and how to set it up:

Gem-EI: A Sentiment-Aware Conversational Bot
This project is a Flask-based web application that interacts with users through a chatbot named Gem-EI. The bot is powered by Google's Gemini Generative AI and is designed to analyze user sentiment, encourage positive conversations, and provide emotional support, especially for users feeling low or depressed. Gem-EI offers personalized responses and attempts to uplift the user's mood through conversation.

Features
Sentiment-aware responses based on user input.
Stores chat history (latest 10 conversations) for context and session continuity.
Uses Google's Gemini Generative AI for generating human-like conversations.
Generates random pastel colors for the UI to enhance user experience.
Handles sensitive topics with empathy and aims to divert users from negative thoughts.
Flask-based web app with an interactive frontend using HTML and CSS.
Requirements
Python 3.x
Flask
dotenv
google-generativeai (for interacting with Google's Gemini API)
Installation
1. Clone the Repository
First, clone this repository to your local machine:

bash
Copy code
git clone https://github.com/PiyushVIT346/Chat-Gemi_E.git
cd Chat-Gemi_E
2. Set Up a Virtual Environment (Optional but Recommended)
It is recommended to create a virtual environment to manage dependencies:

bash
Copy code
python -m venv venv
source venv/bin/activate  # On Windows use `venv\Scripts\activate`
3. Install Dependencies
Install the required packages:

bash
Copy code
pip install -r requirements.txt
4. Set Up Environment Variables
Create a .env file in the root directory of the project and add your Google API key as follows:

makefile
Copy code
GOOGLE_API_KEY=your-google-api-key-here
5. Run the Application
You can now run the Flask application:

bash
Copy code
python app.py
This will start the development server. By default, the app will be available at http://127.0.0.1:5000.

6. Access the Web Application
Open a web browser and navigate to:

arduino
Copy code
http://127.0.0.1:5000
Project Structure
bash
Copy code
.
├── app.py                 # Main Flask application file
├── templates/
│   └── index.html         # HTML template for the chat interface
├── static/
│   └── css
      └──style.css          # CSS file for styling
    └──js
      └──script.js          # JS file 
     
├── .env                   # Environment variables (not in the repo, to be created)
├── requirements.txt       # Python dependencies
├── README.md              # Documentation
Usage
On visiting the home page, users can type in messages, and Gem-EI will respond with empathetic, sentiment-aware replies.
The chat history is stored in the session and refreshed for the latest 10 messages.
If the user asks about themselves, the bot can reference a brief description stored in memory, making the conversation more personalized.
Example Prompts
"I had a bad day at school."
"I'm not feeling good enough."
"Thank you for helping me."
Customization
You can modify the prompt variable in app.py to change how the bot responds to different user emotions and questions.
The pastel color scheme for the chat UI can be adjusted in the get_random_pastel_color() function.
