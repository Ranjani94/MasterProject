## Webapp for Master Project - Artificial Intelligence Enabled Image Generation From Text

### Steps to install Virtualenv:

- pip install virtualenv
- virtualenv env

Steps to run:

- source env/bin/activate
- export FLASK_APP=main.py
- export FLASK_ENV=development (to enable to debug mode in development environment)
- flask run


app.yaml and appengine_config.py - these files are used to deploy the web application using Google App engine in GCP

Steps to deploy the webapp:

- Go to google cloud platform console
- create new project
- install google cloud SDK in your local machine
- make sure env in activated
- pip install -t lib -r requirements.txt [-t lib: This flag copies the libraries into a lib folder, which uploads to App Engine during deployment. -r requirements.txt: Tells pip to install everything from requirements.txt]
- gcloud app deploy [specify the ProjectID which is given in GCP console after creating new project]
- "your project id".appspot.com [check the URL in browser]
