# Chatbot Deployment with Flask and JavaScript

In this tutorial we deploy the chatbot we created in [this](https://github.com/Rohithchowk/CBITchatbot.git) tutorial with Flask and JavaScript.

This gives  deployment option:
- Serve only the Flask prediction API. The used html and javascript files can be included in any Frontend application (with only a slight modification) and can run completely separate from the Flask App then.

## Initial Setup:
This repo currently contains the starter files.

Clone repo and create a virtual environment
```
$ git clone https://github.com/python-engineer/chatbot-deployment.git
$ cd chatbot-deployment
$ python3 -m venv venv
$ . venv/bin/activate
```
Install dependencies
```
$ (venv) pip install Flask torch torchvision nltk
```
Install nltk package
```
$ (venv) python
>>> import nltk
>>> nltk.download('punkt')
```
Modify `intents.json` with different intents and responses for your Chatbot

Run
```
$ (venv) python train.py
```
This will dump data.pth file. And then run
the following command to test it in the console.
```
$ (venv) python chat.py
```

Now for deployment follow my tutorial to implement `app.py` and `app.js`.


## Deployment Link

[chatbot Link](http://chandra76768.pythonanywhere.com/)

The chatbot gives info about our college CBIT , its placements , packages , clubs ,events ,faculty and thier url links , and also information related to  IT department 
