http://localhost:80/     webapp

## Workflows
Update config.yaml
Update schema.yaml
Update params.yaml
Update the entity
Update the configuration manager in src config
Update the components
Update the pipeline
Update the main.py
Update the app.py


How to run?
STEPS:
Clone the repository
https://github.com/Dhach123/End-to-end-Machine-Learning-Project-with-MLflow


STEP 01- Create a conda environment after opening the repository
source ~/anaconda3/etc/profile.d/conda.sh
 virtualenv mlproj
conda activate mlproj
. mlproj/scripts/activate  

1)python -m venv mlproj   old
2)mlproj\Scripts\activate  old  

STEP 02- install the requirements
pip install -r requirements.txt


# Finally run the following command
python app.py

Now
open up you local host and port


# MLflow
DOCUMENT https://mlflow.org/docs/latest/index.html

# Command for MLFLOW
mlflow ui

# dagshub

MLFLOW_TRACKING_URI=https://dagshub.com/Dhach123/End-to-end-Machine-Learning-Project-with-MLflow.mlflow
MLFLOW_TRACKING_USERNAME=xxx
MLFLOW_TRACKING_PASSWORD=xxx
python script.py


Run this to export as env variables:


export MLFLOW_TRACKING_URI=https://dagshub.com/Dhach123/End-to-end-Machine-Learning-Project-with-MLflow.mlflow

export MLFLOW_TRACKING_USERNAME=xxx 

export MLFLOW_TRACKING_PASSWORD=xxx



AZURE-CICD-Deployment-with-Github-Actions

STEP1- CONTAINER REGISTRIES:
salesbigmart
Save pass:
xxxxxxx

STEP2- WEB APP FOR CONTAINERS

Run from terminal:
docker build -t salesbigmart.azurecr.io/mltest:latest .

docker login salesbigmart.azurecr.io   WINPTY

docker push salesbigmart.azurecr.io/mltest:latest

Deployment Steps:

Build the Docker image of the Source Code

Push the Docker image to Container Registry

Launch the Web App Server in Azure

Pull the Docker image from the container registry to Web App server and run

Deployement done. 