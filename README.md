# OpenAI workshop 
Created by: [Denise Schlesinger](https://www.linkedin.com/in/deniseschlesinger/) and [Vlad Feigin](https://www.linkedin.com/in/vladifeigin/) 

⚡ Build OpenAI applications to search your own data ⚡
This agenda covers a range of topics, from the basics of LLMs and GPT to more advanced topics like prompt engineering and embeddings. The labs provide hands-on experience with OpenAI, including connecting to the platform, creating prompts, and working with embeddings. 


## Requirements
For this workshop you MUST have the following:

## Requirements
- VsCode
- Python 3.7
- A virtual environment tool (venv)
- An Azure account 
- An active Azure OpenAI account with 2 deployed models see below

## Preparation

## OpenAI subscription and deployments
* Create an Azure OpenAI account
* Create 'gpt-35-turbo', 'text-davinci-003' and 'text-embedding-ada-002' deployments

### VsCode
* Install [Visual Studio Code](https://code.visualstudio.com/)

### Python
* Install [Python 3.7](https://www.python.org/downloads/release/python-31011/)

### Python3 Virtualenv Setup
*  Installation
        To install virtualenv via pip run:
            $ pip3 install virtualenv
* Creation of virtualenv:
    - Windows
    $ python -m virtualenv venv (in the openAI workshop directory)
    - Mac
    $ virtualenv -p python3 <desired-path>

    Activate the virtualenv:
    $ source <desired-path>/bin/activate

    Deactivate the virtualenv:
    $ deactivate

#### Python3 Virtualenv Setup
*  Installation
        To install virtualenv via pip run:
            $ pip3 install virtualenv
* Creation of virtualenv:
    - Windows
    $ python -m virtualenv venv (in the openAI workshop directory)
    - Mac
    $ virtualenv -p python3 <desired-path>

### Install all libraries in your virtual environment
* Activate the environment
    Windows:
        .\venv\Scripts\activate.ps1
    Mac:
    $ source ./venv/bin/activate

* Make sure you have the requirements installed in your Python environment using `pip install -r requirements.txt`.


# IMPORTANT!
### Setup environment variables
* Rename the '.env.template' file to '.env' and modify all the endpoints and api keys for all openai deployments as follows:
```
OPENAI_DEPLOYMENT_ENDPOINT ="<your openai endpoint>" 
OPENAI_API_KEY = "<your openai api key>"
OPENAI_DEPLOYMENT_NAME = "<your gpt35 deployment name>"
OPENAI_DEPLOYMENT_VERSION = "<gpt35 api version>"
OPENAI_MODEL_NAME="<gpt35 model name>"

OPENAI_ADA_EMBEDDING_DEPLOYMENT_NAME = "<your text embedding ada deployment name>"
OPENAI_ADA_EMBEDDING_MODEL_NAME = "<your text embedding ada model name>"

OPENAI_DAVINCI_EMBEDDING_DEPLOYMENT_NAME = "<your text embedding ada deployment name>"
OPENAI_DAVINCI_EMBEDDING_MODEL_NAME = "<your da vinci model name>"

```