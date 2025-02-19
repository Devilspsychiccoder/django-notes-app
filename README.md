# Simple Notes App for Kubernetes 
This is a simple notes app built with React and Django.

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

## Nginx

Install Nginx reverse proxy to make this application available

`sudo apt-get update`
`sudo apt install nginx`
