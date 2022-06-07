# Managing the end-to-end machine learning lifecycle with MLFlow

This Repository contains the resources for my tutorial **"Managing the end-to-end machine learning lifecycle with MLFlow"** at pyData/pyCon Berlin 2019.

# Basic setup

## Setup the environment
- clone this repository
- **with virtualenv (recommended)**
  - install virtualenv: `pip install virtualenv`
  - create a new environment: `virtualenv mlflow_tutorial`
  - activate the environment: `source mlflow_tutorial/bin/activate`
  - run `pip install -r requirements.txt`
  
- **with pipenv** 
  - install pipenv: `pip install pipenv`
  - run `pipenv install` in the directory of the Pipfile
  - activate the environment by `pipenv shell`

## Launch MLFlow Server
```sh
mlflow server --backend-store-uri mlruns/ --default-artifact-root mlruns/ --host 0.0.0.0 --port 5000
```
![mlflow](https://user-images.githubusercontent.com/105429462/172399024-3436c294-67fd-4c7d-b27f-bba131c7b972.PNG)

## The notebook
- Get the `hands_on_example.ipynb`
- run `jupyter notebook`

# Advanced setup

## Setup the environment
- install postgresql: `sudo apt-get install postgresql postgresql-contrib postgresql-server-dev-all`
