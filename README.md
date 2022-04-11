# Psychiatrist ChatBot
## COSC 310 Software Engineering
### Individual Project 

------

### Local Environment Setup

#### Install Dependencies 

We still need the dependencies from A3 for this revision to work. I will leave the previous dependencies here and add some more after. 

`pip install nltk`

`pip install numpy`

`pip install keras`

`pip install tensorflow`

`pip install spacy`

download spacy model

`python -m spacy download en_core_web_sm`

When first running the program, it may ask you to download certain NTLK packages. The only way I found I could download them was by running the code below:

```python
import nltk
import ssl

try:
    _create_unverified_https_context = ssl._create_unverified_context
except AttributeError:
    pass
else:
    ssl._create_default_https_context = _create_unverified_https_context

nltk.download()
```

Link to source can be found here: https://stackoverflow.com/questions/38916452/nltk-download-ssl-certificate-verify-failed


### For the new Individual Assignment

'pip install googletrans'

'pip3 install wikipedia-api'


#### Train ChatBot

To train the chatbot you can run the file `app/chatbot/train.py`

#### Use ChatBot

To use the chatbot you can run the file `app/chatbot/chatbot_app.py`

------

### List of Features (for A3) 

#### Google Translate API integration

Now the chatbot can communicate in over 100+ different languages using Google Translate. More documentation plus a list of supported languages can be found here 

https://cloud.google.com/translate

### Wikipedia API integration

Now when the chatbot suggests a potential diagnosis, it will give a summary about the disorder from wikipedia as well with a link so the client can find out more about thier potential diagnosis. 


