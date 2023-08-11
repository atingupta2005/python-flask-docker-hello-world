# Simple Python Flask Dockerized Application

### Clone this repo
```
ssh atingupta2005@172.190.40.220
clear
cd
git clone https://github.com/atingupta2005/python-flask-docker-hello-world
cd ~/python-flask-docker-hello-world
```

### Review the files
```
clear
cd ~/python-flask-docker-hello-world
cat app.py
cat requirements.txt
cat Dockerfile
```

### Build the image using the following command

```bash
cd ~/python-flask-docker-hello-world
docker build -t simple-flask-app:latest .
```

### Run the Docker container using the command shown below.

```bash
docker run -d -p 5000:5000 simple-flask-app
```

### Note
 - The application will be accessible at http:127.0.0.1:5000
