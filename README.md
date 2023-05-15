# myproject

Django Web Application with Docker and Kubernetes
This is a simple web application created using Python Django, Docker and Kubernetes, with automation setup using Jenkins.

## Features
- Django web application with basic user interface
- Docker containerization for the application
- Automated build and deployment using Jenkins
- Deployment to a Kubernetes cluster
## Prerequisites
To run this application, you must have the following installed:

- Python 3
- Docker
- Kubernetes
- Jenkins

## Installation
Follow the steps below to install and run the application:

1. Clone the repository to your local machine using git clone.
2. Change directory into the project folder using cd.
3. Build the Docker image using docker build -t <image-name> ..
4. Run the Docker container using docker run -p 8000:8000 <image-name> to start the Django web application.
5. Open your web browser and go to http://localhost:8000 to view the application.
  
## Jenkins Automation
The Jenkins automation for this project includes the following steps:

1. Pull the latest code from the GitHub repository.
2. Build a Docker image of the application.
3. Push the Docker image to DockerHub or another container registry.
4. Deploy the application to a Kubernetes cluster.
  
## Deployment
To deploy the application to a Kubernetes cluster, follow these steps:

1. Ensure that you have a Kubernetes cluster set up and running.
2. Update the Kubernetes deployment file with the name of the Docker image you pushed to DockerHub or another container registry.
3. Apply the deployment file using kubectl apply -f <deployment-file> to deploy the application to the cluster.
  
## Conclusion
This project demonstrates a simple Django web application that has been containerized using Docker and deployed to a Kubernetes cluster with automation set up using Jenkins. With these tools and technologies, you can easily build and deploy web applications in a scalable and efficient manner.
