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
docker login -u <dockeraccountname>
```
3. Build the app
```
docker build -t notes-app .
```
4. Tag the Image
```
docker image tag notes-app-k8s:latest thatgeekcontainer/notes-app-k8s:latest
```
3. Run the app
```
docker run -d -p 8000:8000 notes-app:latest
```

## Nginx

Install Nginx reverse proxy to make this application available

`sudo apt-get update`
`sudo apt install nginx`
