# Basic Flask application

Before you begin, ensure that you have the following tools installed on your machine:

- **[kubectl](https://kubernetes.io/docs/reference/kubectl/kubectl/).** You can learn how to install the Kubernetes command-line tool for managing and interacting with your cluster [in Kubernetes’s docs](https://kubernetes.io/docs/tasks/tools/install-kubectl/).
- **[minikube](https://minikube.sigs.k8s.io/docs/).** You can install this tool for running a single-node Kubernetes cluster on your local machine by following [minikube’s documentation](https://minikube.sigs.k8s.io/docs/start/).
- **​​[k3d](https://k3d.io/v5.4.9/).** This is a lightweight wrapper to run k3s, which is a Kubernetes cluster in a Docker container for development purposes.
- **[Git](https://git-scm.com).** [Install this version control system](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git) to manage your application's source code.
- **[Docker](https://www.docker.com).** [Install this platform](https://docs.docker.com/desktop/) to develop, ship, and run applications in containers.
- **[Docker Hub](https://hub.docker.com/signup).** Create a Docker Hub account to host your Docker image.
- **[Skaffold](https://skaffold.dev).** [Download Skaffold](https://skaffold.dev/docs/install/) to automate your development workflow by building, pushing, and deploying applications to Kubernetes clusters.
- **[Garden](https://docs.garden.io).** [Download Garden](https://docs.garden.io/guides/installation) to simplify the management of complex applications with multiple services, dependencies, and environments (make sure you don't install the tool using npm as it's deprecated). This tutorial uses version 0.12.53. 
- **[Google Cloud Platform (GCP)](https://cloud.google.com/gcp/).** For this tutorial, [use GCP’s free trial account](https://developers.google.com/maps/documentation/places/web-service/cloud-setup) with $300 in credits to ensure that you have an account with a project created and billing enabled. 
- **[gcloud CLI](https://cloud.google.com/sdk/docs/install).** This command line tool authenticates with your GCP account.
- **[Helm](https://helm.sh/docs/intro/install/).** You'll use this tool to simplify the process of deploying your Kubernetes application on GCP.

## Run your Flask application with Docker

To run the application with Docker, go to the root directory of the project and use the following commands :

```
docker build -t basic-flask-application .
docker run -p 8080:8080 basic-flask-application
```

Next, open your browser and navigate to [http://localhost:8080/](http://localhost:8080/), and you should see the output of your application. 

![Flask Hello World Application](https://i.imgur.com/LJFRJU8.png)



Have fun !
Author : Lucien Chemaly
