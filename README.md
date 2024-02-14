<div align="center">
  <div id="user-content-toc">
    <ul>
      <summary><h1 style="display: inline-block;">🥔 Potato Disease Classification</h1></summary>
    </ul>
  </div>
  
  <p>Deep Learning Project Using Tensorflow ,Mlflow, DVC, AWS & Flask </p>
    <!-- <a href="https://youtu.be/OWAefZ1vE8I" target="_blank">Demo</a>
    ·
    <a href="https://www.kaggle.com/datasets/arjuntejaswi/plant-village" target="_blank">Data</a>
    ·
    <a href="https://github.com/Hamagistral/Potato-Disease-Classification/issues" target="_blank">Request Feature</a>
</div> -->

![alt text](image.png)

## 🎯 Goal 

The goal of this project is to help farmers diagnose their crops. This project uses image classification using CNN architecture with Tensorflow to detect potato plant diseases, deployed to GCP and used in a web frontend app made with React.


## 💾 Dataset Used  

This data contains three datasets that contains photos of potato leaves. One dataset contains `Healthy` potato leaves, `Early Blight` and `Late Blight`.

More info about dataset can be found here :

- Github - https://github.com/alokpandey098/internship_projects/raw/main/Potatoes-leaf.zip



## 🛠️ Technologies Used

![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)
![Jupyter](https://img.shields.io/badge/Made%20with-Jupyter-orange?style=for-the-badge&logo=Jupyter)
![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white)
![MlFlow](https://img.shields.io/badge/Mlflow-3670A0?style=for-the-badge&logoColor=ffdd54)
![DVC](https://img.shields.io/badge/DVC-orange?style=for-the-badge)

![AWS](https://img.shields.io/badge/AWS-569A31?style=for-the-badge&logo=AWS&logoColor=ffdd54)

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
    - Save the URI: 730335511510.dkr.ecr.ap-south-1.amazonaws.com/wine-check

	
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

    AWS_ECR_LOGIN_URI = demo>>  566373416292.dkr.ecr.ap-south-1.amazonaws.com

    ECR_REPOSITORY_NAME = simple-app





[LinkedIn](www.linkedin.com/in/alok-kumar-11075b252) •
[Gmail](kalok0575@gmail.com) •