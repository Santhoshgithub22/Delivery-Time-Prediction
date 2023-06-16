# Zomato Delivery Time Prediction

## Virtual Environment
#### ---------------------------------------
Creating a new virtual environment for zomato delivery time prediction project

```
conda create -p venv python==3.8
```

## Requirement.txt
#### ---------------------------------------

Creating a requirements text file, By using requirement.txt file, we can able to install all packages which is required for this project

```
pip install -r requirements.txt
```

## Setup.py
#### ---------------------------------------

Creating a setup.py file, Whenever we want to convert this project into packages, That type we probably use this setup.py file

```
python setup.py
```

## Creating source folder
#### ---------------------------------------
Inside this source folder my entire Machine Learnig life cycle should be run.  Whenever we create a folder always we should create a __init__.py file.  Because, this source folder also a package, we should able to reuse it, install it somewhere else.

## Creating logger.py, exception.py, utils.py Files
#### -----------------------------------------------------------------------------------

logger.py file for logging, exception.py file for to handle the exceptions and utils.py file basically means any generic functionality probably that I want to create for this entire project.

## Creating Notebooks folder
#### -------------------------------------------------
EDA, Feature Engineering, data transformation, and all.  We have to do somewhere else, so for that I hae created the notebooks folder, and inside this folder, I have data folder for dataset, EDA python notebook file and model python notebook file.

I dont want to go this folder as a package.

## Creating components folder inside source folder
#### ----------------------------------------------------------------------------------------
This folder is a super important folder, whenever we create a project we have to follow a life cycle.

```

The life cycle divided into 6 parts. i.e,

    1. Data Cleaning,
    2. Data Ingestion,
    3. Data Transformation,
    4. Model Training,
    5. Model Evaluation,
    6. Deployment

    LIFE CYCLE OF PROJECT:
    _____________________________________________________________________________________
    | Input                 | ----> | Processing        | ----> | Output                |
    |_______________________|_______|___________________|_______|_______________________|
    |Raw Data               | ----> |Data Cleaning      | ----> |Clean Data             |
    |Clean Data             | ----> |Data Ingestion     | ----> |Train & Test Split Data|
    |Train & Test Split Data| ----> |Data Transformation| ----> |Train & Test Data      |
    |Train & Test Data      | ----> |Model Training     | ----> |Pickle File            |
    |Pickle File            | ----> |Model Evaluation   | ----> |Better Output          |
    |Better Output          | ----> |Deployment         | ----> |Best Product           |
    |_______________________|_______|___________________|_______|_______________________|

```

## Creating pipeline folder inside source folder
#### ----------------------------------------------------------------------------------------
Whenever we creating a project, we should train the model and get prediction from the model, so for that we should create pipeline inside the pipeline folder, one is training_pipeline folder and another one is prediction_pipeline folder.  Also created a python file (__init__.py).  Because, this source folder also a package, we should able to reuse it, install it somewhere else.

    1. Training Pipeline ----> In life cycle training pipeline will go to data cleaning and come out from the deployment.

    2. Prediction Pipeline ----> Whatever model I have created, this prediction pipeline will take a input & give it to the model & model will give a output.

## Artifacts folder
#### -----------------------------------
The model output will go to the artifacts folder, but the folder will created by code, not manually.