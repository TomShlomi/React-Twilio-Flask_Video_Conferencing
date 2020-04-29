# React-Twilio-Flask_Video_Conferencing
 Runs a Twilio video conference on localhost. Uses a Flask backend and React frontend.
 
 How to install:
 
 1: Clone this repository.
 
 2: Navigate to React-Twilio-Flask_Video_Conferencing in the command terminal and enter "npm install" to install dependencies.
 
 3: Navigate to flask-twilio-video and enter "python -m venv venv" in the command terminal to install a virtual environment.
 
 4: Enter "venv\Scripts\activate", then "pip install flask python-dotenv", and then "pip install twilio" into the command terminal.
 
 5: If you do not have one, create a [twilio account](https://twilio.com). Use your account to create a twilio api key.
 
 6: Copy the .env.example files in React-Twilio-Flask_Video_Conferencing and flask-twilio-video into .env files. Fill them with the details of your api key.
 
 7: In React-Twilio-Flask_Video_Conferencing, run "yarn start-api". The backend should now be running.
 
 8: Open a new command terminal, go to React-Twilio-Flask_Video_Conferencing, and type "npm run dev" in the command window. localhost:3000 should open in a browser. You should now be able to enter a room and see yourself.
 
 9: For people to use this service from another computer, you will need a https address. To do so, [install ngrok](https://ngrok.com/download). Open the folder where ngrok.exe is and enter "ngrok http 3000 -host-header="localhost:3000" into the command terminal. Copy the https address. Now anyone can access the web service by navigating to that address.
