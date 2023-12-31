# End-to-end-Machine-Learning-Project-with-MLflow

```
MLflow model
```

![Screenshot (13)](https://github.com/saisubhasish/End-to-end-Machine-Learning-Project-with-MLflow/assets/102937478/24bc2338-3853-4530-9aeb-b479f9473f3e)

```
AWS deployed app
```
![Screenshot (18)](https://github.com/saisubhasish/End-to-end-Machine-Learning-Project-with-MLflow/assets/102937478/e42b5e99-5e57-490b-ad5c-9cd2c021f0f8)
![Screenshot (19)](https://github.com/saisubhasish/End-to-end-Machine-Learning-Project-with-MLflow/assets/102937478/d27fd4fd-6b7e-4718-957c-ad01781e64ba)
![Screenshot (17)](https://github.com/saisubhasish/End-to-end-Machine-Learning-Project-with-MLflow/assets/102937478/b7485213-c066-4b45-b4fc-ccf9755f30e8)

## Workflows

1. Update config.yaml
2. Update schema.yaml
3. Update params.yaml
4. Update the entity
5. Update the configuration manager in src config
6. Update the components
7. Update the pipeline 
8. Update the main.py
9. Update the app.py



# How to run?
### STEPS:

Clone the repository

```bash
https://github.com/saisubhasish/End-to-end-Machine-Learning-Project-with-MLflow
```
### STEP 01- Create a conda environment after opening the repository

```bash
conda create -n mlproj python=3.8 -y
```

```bash
conda activate mlproj
```


### STEP 02- install the requirements
```bash
pip install -r requirements.txt
```


```bash
# Finally run the following command
python app.py
```

Now,
```bash
open up you local host and port
```



## MLflow

[Documentation](https://mlflow.org/docs/latest/index.html)


##### cmd
- mlflow ui

### dagshub
[dagshub](https://dagshub.com/)

MLFLOW_TRACKING_URI=https://dagshub.com/saisubhasish/End-to-end-Machine-Learning-Project-with-MLflow.mlflow \
MLFLOW_TRACKING_USERNAME=saisubhasish \
MLFLOW_TRACKING_PASSWORD=8391a403cca1692284416014c9589f715588782e \
python script.py

Run this to export as env variables:

```bash

export MLFLOW_TRACKING_URI=https://dagshub.com/saisubhasish/End-to-end-Machine-Learning-Project-with-MLflow.mlflow

export MLFLOW_TRACKING_USERNAME=saisubhasish 

export MLFLOW_TRACKING_PASSWORD=8391a403cca1692284416014c9589f715588782e

```



# AWS-CICD-Deployment-with-Github-Actions

## 1. Login to AWS console.

## 2. Create IAM user for deployment

	#with specific access

	1. EC2 access : It is virtual machine

	2. ECR: Elastic Container registry to save your docker image in aws


	#Description: About the deployment

	1. Build docker image of the source code

	2. Push your docker image to ECR

	3. Launch Your EC2 

	4. Pull Your image from ECR in EC2

	5. Lauch your docker image in EC2

	#Policy:

	1. AmazonEC2ContainerRegistryFullAccess

	2. AmazonEC2FullAccess

	
## 3. Create ECR repo to store/save docker image
    - Save the URI: 922583229771.dkr.ecr.us-east-1.amazonaws.com/mlflowproject

	
## 4. Create EC2 machine (Ubuntu) 

## 5. Open EC2 and Install docker in EC2 Machine:
	
	
	#optinal

	sudo apt-get update -y

	sudo apt-get upgrade
	
	#required

	curl -fsSL https://get.docker.com -o get-docker.sh

	sudo sh get-docker.sh

	sudo usermod -aG docker ubuntu

	newgrp docker
	
# 6. Configure EC2 as self-hosted runner:
    setting>actions>runner>new self hosted runner> choose os> then run command one by one


# 7. Setup github secrets:

    AWS_ACCESS_KEY_ID=

    AWS_SECRET_ACCESS_KEY=

    AWS_REGION = us-east-1

    AWS_ECR_LOGIN_URI = 922583229771.dkr.ecr.us-east-1.amazonaws.com

    ECR_REPOSITORY_NAME = mlflowproject




## About MLflow 
MLflow

 - Its Production Grade
 - Trace all of your expriements
 - Logging & tagging your model


