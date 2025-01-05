# Ovewview of the Project

## Project: ALEX_The_Chatbot

**Alex the Chatbot** is an intelligent and interactive chatbot built for a restaurant website to streamline food ordering and delivery services. Powered by Dialogflow and FastAPI, Alex enables users to effortlessly perform the following actions through natural language conversations:
- Place New Orders: Users can explore the menu and create new food orders.
- Track Existing Orders: Stay updated on the status of ongoing orders.
- Modify Orders: Remove specific items or quantities from the order dynamically.
The backend is built using FastAPI, which connects seamlessly to a MySQL database to manage and persist order data. The chatbot leverages Dialogflow's natural language processing (NLP) capabilities to understand user queries and provide accurate responses.

## Key Features:
- Conversational Ordering: Simplifies the food ordering process with a user-friendly chat interface.
- Dynamic Order Updates: Allows users to modify orders by removing specific items or quantities.
- Real-time Tracking: Enables users to check the current status of their orders.
- Scalable Backend: Built with FastAPI and connected to MySQL for reliable and scalable order management.

<p align="center">
  <img src="https://github.com/user-attachments/assets/4534b5c8-fc11-41b0-a77d-a26eaf7868bb" width="90%" />
</p>

<p align="center">
  <img src="https://github.com/user-attachments/assets/7c53fe30-41e6-484e-9732-5ce055c3bbc5" width="33%" />
  <img src="https://github.com/user-attachments/assets/68729158-bf47-4733-aeb7-3393d5ed6851" width="33%" />
  <img src="https://github.com/user-attachments/assets/ab625756-7508-4d75-a306-051a0a1742a9" width="33%" />
</p>
<p align="center">
  <img src="https://github.com/user-attachments/assets/3c31c50c-343b-4bcd-bbe0-1bf9dc424331" width="24.5%" />
  <img src="https://github.com/user-attachments/assets/805c8e54-af42-4663-8a5f-e0721b770fc5" width="24.5%" />
  <img src="https://github.com/user-attachments/assets/c742f137-f653-4ea5-b65d-18af52d18f3f" width="24.5%" />
  <img src="https://github.com/user-attachments/assets/c0dcc7a2-c044-41b2-9297-9bd37933ce60" width="24.5%" />
</p>


## Directory structure
backend: Contains Python FastAPI backend code
db: contains the dump of the database. you need to import this into your MySQL db by using MySQL workbench tool
dialogflow_assets: this has training phrases etc. for our intents
frontend: website code

## Install these modules
pip install mysql-connector
pip install "fastapi[all]"

OR just run pip install -r backend/requirements.txt to install both in one shot

## To start fastapi backend server
1. Go to backend directory in your command prompt
2. Run this command: uvicorn main:app --reload

## ngrok for https tunneling
1. To install ngrok, go to https://ngrok.com/download and install ngrok version that is suitable for your OS
2. Extract the zip file and place ngrok.exe in backend folder.
3. Open windows command prompt, go to that folder and run this command: ngrok http 80000
4. Paste the generated URL from command prompt to DialogFlow Fullfillments 

NOTE: ngrok can timeout. you need to restart the session if you see session expired message.
