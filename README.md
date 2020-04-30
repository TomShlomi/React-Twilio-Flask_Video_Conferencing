# React-Twilio-Flask_Video_Conferencing
Runs a Twilio video conference on localhost. Uses a Flask backend and React frontend. This is a work in progress, so there may be some bugs. The installation instructions are for Windows. If you are not using Windows, replace "venv\scripts\activate" with "venv/bin/activate" and go into package.json and replace "venv/Scripts/flask" with "venv/bin/flask". No tests have been run on non-Windows machines, so other changes might be necessary.
 
 Requirements:
 [node.js](https://nodejs.org/en/download/)
 [yarn](https://classic.yarnpkg.com/en/docs/install/#windows-stable)
 [Python 3](https://www.python.org/downloads/)
 [ngrok](https://ngrok.com/download)
 [A twilio account](www.twilio.com/referral/Tyy8tr)
 
 Installation Instructions:
 
 1: Clone this repository.
 
 2: Navigate to React-Twilio-Flask_Video_Conferencing in the command terminal and enter "npm install" to install dependencies.
 
 3: Navigate to flask-twilio-video and enter "python -m venv venv" in the command terminal to install a virtual environment.
 
 4: Enter "venv\Scripts\activate", then "pip install flask python-dotenv", and then "pip install twilio" into the command terminal.
 
 5: Create a [twilio api key](https://www.twilio.com/console/video/project/api-keys).
 
 6: Edit the two .env.template files in React-Twilio-Flask_Video_Conferencing and \flask-twilio-video: Fill them with the details of your api key. Save them as ".env".
 
 Usage Instructions:
 
 1: In React-Twilio-Flask_Video_Conferencing, "yarn start-api". The backend should now be running.
 
 2: Open a new command terminal, go to React-Twilio-Flask_Video_Conferencing, and type "npm run dev" in the command window. localhost:3000 should open in a browser. Enter a name and room to create or join a video conference. You should now see yourself.
 
 3: For people to use this service from another computer, you will need a https address. Open the folder containing ngrok.exe and enter "ngrok http 3000 -host-header="localhost:3000" into the command terminal. Copy the https address. Now anyone can access the web service by navigating to that address. To join an existing video conference, the same room name is required. Note that all user names must be unique.
