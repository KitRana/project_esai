# Project ESAI  
<!-- forthebadge -->
[![forthebadge](https://forthebadge.com/images/badges/made-with-python.svg)](https://forthebadge.com)
[![forthebadge](https://forthebadge.com/images/badges/built-with-love.svg)](https://forthebadge.com)  
[![forthebadge](https://forthebadge.com/images/badges/uses-js.svg)](https://forthebadge.com) [![forthebadge](https://forthebadge.com/images/badges/uses-html.svg)](https://forthebadge.com)
[![forthebadge](https://forthebadge.com/images/badges/uses-css.svg)](https://forthebadge.com)  
### And so much more!

## About
Project ESAI is an experiment in contextual AI.  The Emergency Service Artificial Intelligence (ESAI) system aims to provide chat and voice based assistance to emergency response situations.  The system would act as a supplement to current 911 operations.  ESAI would be the first line of connection for people seeking emergency assistance through a web or mobile application.  ESAI would connect to a user, ask what type of emergency service is needed (ie. police, fire, or ems) and 

## Machine Learning

ESAI is built on a new open source AI framework called [Rasa].  While there are plenty of chatbots deployed these days, most use state-machines and are powered but pre-defined rules which are great until they need to be scaled.  Rasa uses a machine learning approach to dialogue management which allows users to have natural conversations with AI assistants.  The system uses NLU models for intent classification and entity extraction, which allows the computer to understand the actual context of the conversation rather than pre-programmed rules.  Machine learning models are also used to predict responses to the users.  This is the future of the AI assistant, and ESAI aims to bring these methods to triage emergency response.  

## Screenshots
<img src="./screenshots/esai_response1.gif" width="auto" height="450" title= "police response 1" alt= "police response 1"/>
<img src="./screenshots/esai_response2.gif" width="auto" height="450" title= "police response 2" alt= "police response 2"/>  
<img src="./screenshots/esai_chitchat.gif" width="auto" height="450" title= "chitchat" alt= "chitchat"/>  

## Future Updates
* Docker server deployment - the system can then be accessed from anywhere
* Custom Actions  
    * Retrieve emergency reponse facility locations
    * Ask user for location with a browser prompt (ie. `navigator.geolocation.getCurrentPosition()`)
    * Conversation clear button
    * Image upload button
    * Display images in window


## Sources
The websocket chat widget featured in the screenshots is sourced from [Rasa Webchat].  
Additional testing is being done with [Chatroom] and [Chatbot-Widget].  

Thank you to all the amazing developers and Rasa community for all your help!  

<!-- Links -->
[Rasa]:https://www.rasa.ai 
[Rasa Webchat]:https://github.com/botfront/rasa-webchat
[Chatroom]:https://github.com/scalableminds/chatroom
[Chatbot-Widget]:https://github.com/JiteshGaikwad/Chatbot-Widget
