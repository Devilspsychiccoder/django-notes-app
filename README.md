# Simple Notes App for Kubernetes.
This is a simple notes app built with React and Django. This is make In kind Cluster, Tailor it according to your environment

## Requirements
1. Python 3.9
2. Node.js
3. React

## Installation
1. Clone the repository
```
git clone https://github.com/Devilspsychiccoder/django-notes-app.git
```
2. Login to Docker
```
docker login -u thatgeekcontainer
```
3. Build the app
```
docker build -t notes-app .
```
4. Tag the Image
```
docker image tag notes-app-k8s:latest thatgeekcontainer/notes-app-k8s:latest
```
5. Push the Docker Image to your Docker Hub Account
```
docker push thatgeekcontainer/notes-app-k8s:latest
```
6. Run the app
```
k apply -f .
```

7. Make sure you portforward to make the application running
```
kubectl port-forward service/notes-app-service 8000:8000 --address=0.0.0.0 &
```
